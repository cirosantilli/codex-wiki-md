<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\to^*$ for the [reflexive closure](../../../../../reflexive-closure.md) of the [transitive closure of a relation](../../../../../transitive-closure-relation.md) $\to$, and $\leftrightarrow^*$ for its generated [equivalence relation](../../../../../equivalence-relation.md). The [diamond property](../../../../../diamond-property-of-a-reduction-relation.md) requires every pair $a\to b,a\to c$ to admit a one-step join $b\to d\leftarrow c$. The [Church-Rosser property](../../../../../church-rosser-property-of-a-reduction-relation.md) requires a possibly longer join whenever $b\leftrightarrow^*c$. Equivalently, every pair of finite reductions with the same source has a common finite reduct. Identity steps may be included in the diamond convention without affecting the counterexample below.

Let $A=(\lambda z.z)y$ and consider the [lambda term](../../../../../lambda-term.md) $M=(\lambda x.xx)A$. Contracting its outer [beta-redex](../../../../../beta-redex.md) gives $AA$, whereas contracting the inner [beta-redex](../../../../../beta-redex.md) gives $(\lambda x.xx)y$. The only one-step reducts of $AA$ are $yA$ and $Ay$; the other branch has the sole one-step reduct $yy$. These terms are different even under [alpha equivalence](../../../../../alpha-equivalence.md). Thus **one-step beta reduction has no diamond property**. Both branches do reach $yy$ by finite [beta reduction](../../../../../beta-reduction.md).

For the positive result, use [parallel beta reduction](../../../../../parallel-beta-reduction.md) $\Rightarrow$, with rules

$$
x\Rightarrow x,\qquad \frac{P\Rightarrow P'}{\lambda x.P\Rightarrow\lambda x.P'},\qquad \frac{P\Rightarrow P'\quad Q\Rightarrow Q'}{PQ\Rightarrow P'Q'},\qquad \frac{P\Rightarrow P'\quad Q\Rightarrow Q'}{(\lambda x.P)Q\Rightarrow P'[x:=Q']}.
$$

[Structural induction](../../../../../structural-induction.md), renaming binders to avoid capture, proves the substitution lemma: $P\Rightarrow P'$ and $Q\Rightarrow Q'$ imply $P[x:=Q]\Rightarrow P'[x:=Q']$. Define the [complete development of a lambda term](../../../../../complete-development-of-a-lambda-term.md) by

$$
x^\bullet=x,\qquad (\lambda x.P)^\bullet=\lambda x.P^\bullet,\qquad ((\lambda x.P)Q)^\bullet=P^\bullet[x:=Q^\bullet],
$$

and $(PQ)^\bullet=P^\bullet Q^\bullet$ when the application is not initially a root [beta-redex](../../../../../beta-redex.md). Induction on a parallel derivation, using the substitution lemma in the contracting case, proves

$$
M\Rightarrow N\quad\Longrightarrow\quad N\Rightarrow M^\bullet.
$$

Consequently any two parallel reducts have the common successor $M^\bullet$. The ordinary one-step relation is included in the parallel relation, and every parallel step expands into finitely many ordinary steps; their finite closures therefore coincide. A finite grid of parallel diamonds joins any two finite parallel reductions. Finally a finite zigzag of forward and backward reductions can be joined inductively using that confluence. Hence **beta reduction has the Church-Rosser property**, although its individual steps do not have the [diamond property](../../../../../diamond-property-of-a-reduction-relation.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
