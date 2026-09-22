<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [lambda term](../../../../../lambda-term.md) is built recursively as a variable $x$, an application $MN$, or a [lambda abstraction](../../../../../lambda-abstraction.md) $\lambda x.M$. Application associates to the left and abstraction binds occurrences of its variable. We identify consistent renamings of bound variables by [alpha equivalence](../../../../../alpha-equivalence.md). A [beta reduction](../../../../../beta-reduction.md) contracts $(\lambda x.M)N$ to the [capture-avoiding substitution](../../../../../capture-avoiding-substitution.md) $M[x:=N]$, at any subterm. Write $\to_\beta^*$ for finitely many such steps, including none. [Beta equivalence](../../../../../beta-equivalence.md) is the reflexive, symmetric, transitive closure of reduction, so it is represented by a finite zigzag of forward and backward steps.

To prove the [Church-Rosser theorem](../../../../../church-rosser-theorem.md), introduce [parallel beta reduction](../../../../../parallel-beta-reduction.md) $\Rightarrow$ by the four rules

$$
x\Rightarrow x;\qquad M\Rightarrow M'\ \Longrightarrow\ \lambda x.M\Rightarrow\lambda x.M';
$$



$$
M\Rightarrow M',\ N\Rightarrow N'\ \Longrightarrow\ MN\Rightarrow M'N';
$$



$$
M\Rightarrow M',\ N\Rightarrow N'\ \Longrightarrow\ (\lambda x.M)N\Rightarrow M'[x:=N'].
$$

By structural induction every term parallel-reduces to itself. Each ordinary step is a parallel step. Conversely, each parallel step can be performed by an ordinary finite sequence: reduce the displayed subterms recursively, and in the fourth rule contract the root last. Hence $\Rightarrow^*$ and $\to_\beta^*$ are the same relation.

The substitution lemma is

$$
M\Rightarrow M',\ N\Rightarrow N'\ \Longrightarrow\ M[x:=N]\Rightarrow M'[x:=N'].
$$

Prove it by induction on the parallel-reduction derivation for $M$. The variable case separates $M=x$ from other variables; application and abstraction follow from their inductive hypotheses. For abstraction, rename its binder fresh for $x,N,N'$ before substituting. For a contracted redex, choose its binder $y$ distinct from $x$ and fresh for $N,N'$. The substitution identity $P[y:=Q][x:=N]=P[x:=N][y:=Q[x:=N]]$ follows by structural induction with fresh binders; the variable cases use $y\notin FV(N)$, and application and abstraction preserve the identity. Apply the hypotheses to the body and argument, then the parallel contraction rule and this identity. This proves the lemma for every derivation, including simultaneous contractions inside a redex.

Define the [complete development of a lambda term](../../../../../complete-development-of-a-lambda-term.md) by

$$
x^\bullet=x,\qquad (\lambda x.M)^\bullet=\lambda x.M^\bullet,
$$



$$
(MN)^\bullet=\begin{cases}P^\bullet[x:=N^\bullet],&M\text{ is syntactically }\lambda x.P,\\M^\bullet N^\bullet,&\text{otherwise}.\end{cases}
$$

Only a root redex already present in the source application is contracted by this clause; a newly created root redex need not be contracted.

We claim that **$M\Rightarrow N$ implies $N\Rightarrow M^\bullet$**. Induct on the derivation. The variable and abstraction cases are immediate. In the ordinary application rule, use the inductive developments of both components. If its original function is an abstraction, also contract the resulting root redex by the parallel contraction rule; otherwise just use the application rule, even if the reduct has acquired a new root redex. In the contraction rule, the reduct has form $P'[x:=Q']$, and the substitution lemma with $P'\Rightarrow P^\bullet$, $Q'\Rightarrow Q^\bullet$ gives $P'[x:=Q']\Rightarrow P^\bullet[x:=Q^\bullet]$. This establishes the claim.

Consequently, any two parallel reducts $N,P$ of $M$ each parallel-reduce to $M^\bullet$. Thus parallel reduction has the one-step diamond property. Its finite transitive closure is confluent: fill a finite grid of elementary diamonds to join two finite reduction paths from the same term. Since its closure equals ordinary finite [beta reduction](../../../../../beta-reduction.md),

$$
M\to_\beta^*N,\quad M\to_\beta^*P\ \Longrightarrow\ \exists Q:\ N\to_\beta^*Q,\ P\to_\beta^*Q.
$$

A finite conversion zigzag now also has a common reduct, by induction along it. If the next zigzag step points forward from a term already having a common reduct, join its two outgoing paths by confluence; if it points backward, compose the new forward path to that common reduct. The reverse implication is immediate because two paths to a common reduct form a conversion zigzag. This proves

$$
\boxed{M\equiv_\beta N\ \Longleftrightarrow\ \exists Q:\ M\to_\beta^*Q\ \text{and}\ N\to_\beta^*Q.}
$$

A [beta-normal form](../../../../../beta-normal-form.md) contains no beta-redex, so its only finite reduct is itself. If two normal forms are beta-equivalent, their common reduct must equal both. Hence **a term has at most one [beta-normal form](../../../../../beta-normal-form.md) up to [alpha equivalence](../../../../../alpha-equivalence.md)**. The qualification about bound-variable names is essential.

For an example without normal form, take the [Omega combinator](../../../../../omega-combinator.md)

$$
\Omega=(\lambda x.xx)(\lambda x.xx).
$$

Its only redex is the root, and contracting it reproduces $\Omega$. Every finite reduct is therefore $\Omega$, which is not a [beta-normal form](../../../../../beta-normal-form.md). By the theorem it cannot even be beta-equivalent to any normal form.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 87](../../paper-87-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
