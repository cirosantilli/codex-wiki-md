<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The two different term letters in the printed implication must be made consistent; write the indexed step as $M^I\to N^J$. An [indexed lambda term](../../../../../indexed-lambda-term.md) in $\Lambda_\bot^{\mathbb N}$ is a finite [lambda term](../../../../../lambda-term.md) with a bottom constant $\bot$, together with a natural-number index at every subterm occurrence. Equal-looking subterms at different occurrences can have different indices. Bottom here is a constant, not an abbreviation for the divergent [Omega combinator](../../../../../omega-combinator.md).

For $a\subseteq\mathbb N$, write $a_n=a\cap\{0,\ldots,n\}$; in particular $a_0$ can contain zero. Use the [graph model of lambda calculus](../../../../../graph-model-of-lambda-calculus.md) and its pairing code from the preceding solution. If the root index is $n$, interpretation is recursive:

$$
\llbracket x^n\rrbracket_\rho=(\rho(x))_n,\qquad\llbracket\bot^n\rrbracket_\rho=\varnothing,\qquad\llbracket(P^I Q^J)^n\rrbracket_\rho=(\llbracket P^I\rrbracket_\rho\cdot\llbracket Q^J\rrbracket_\rho)_n,
$$



$$
\llbracket(\lambda x.P^I)^n\rrbracket_\rho=\bigl\{\langle k,t\rangle:t\in\llbracket P^I\rrbracket_{\rho[x:=e_k]}\bigr\}_n.
$$

Thus every constructor is clipped at its own occurrence index, not merely at the overall root.

Here are the [indexed beta reduction](../../../../../indexed-beta-reduction.md) rules. In $(\lambda x.P^n)^{m+1}Q^p$, substitute a copy of $Q$ at each free occurrence $x^r$ with that copy's root index lowered to $\min(m,p,r)$. Lower the substituted body's root index further by taking its minimum with $\min(m,n)$; other inherited indices remain unchanged. If the entire body is $x$, this retains the root bound of the inserted argument as well. For an abstraction with index zero, substitute $\bot^0$ for $x$ instead and lower the resulting body root index to zero. The previous root index on the redex application need not be retained. Reduction is allowed in all contexts. Bottom reduction additionally collapses $\bot N$ and $\lambda x.\bot$ to $\bot$; one can collapse the whole maximal abstraction/left-application context in which an occurrence of bottom is at the head. These rules are sensitive to the pairing and cutoff conventions just specified.

To prove semantic monotonicity, first check the finite-witness bounds, writing $a\cdot b$ for graph application:

$$
a_{m+1}\cdot b\subseteq(a\cdot b_m)_m,\qquad a_0\cdot b=(a\cdot\varnothing)_0.
$$

For the first bound, a witness $\langle k,t\rangle\le m+1$ has $t\le m$. If $t>0$, the pairing code is strictly larger than $t$; for $t=0$ the assertion is automatic. Also every member $j$ of $e_k$ satisfies $j<k\le\langle k,t\rangle\le m+1$, hence $j\le m$. So the same witness uses only $b_m$. For the zero-index case the sole possible graph entry is $\langle0,0\rangle=0$, whose finite-input witness is $e_0=\varnothing$.

Let $B=\llbracket Q^p\rrbracket_\rho$ and $f(b)=\llbracket P^n\rrbracket_{\rho[x:=b]}$. A syntax induction gives the indexed substitution equality: replacing $x^r$ by a copy of $Q$ with root $\min(m,p,r)$ interprets that occurrence as $(B_m)_r$, exactly its value when the bound variable receives $B_m$. The body-root change to $\min(m,n)$ clips the resulting body value at $m$. Hence the positive-index contractum has interpretation $(f(B_m))_m$, while the redex before contraction is included in that set by the finite-witness bound. In the zero-index case the contractum interprets as $(f(\varnothing))_0$, equal to the un-clipped application of the zero-indexed abstraction. The old application-root cutoff can only decrease the redex value. Bottom contractions preserve the empty interpretation: the empty graph applied to anything is empty, and abstraction with an everywhere-empty body has empty graph. All surrounding interpretation constructors are monotone. Therefore

$$
\boxed{M^I\to N^J\quad\Longrightarrow\quad\llbracket M^I\rrbracket_\rho\subseteq\llbracket N^J\rrbracket_\rho.}
$$

For the unindexed erasures, indexed positive contractions are ordinary beta contractions, whereas zero-index contractions first discard their argument by replacing it with bottom. Consequently the result contains no new Böhm information:

$$
\boxed{BT(N)\sqsubseteq BT(M),}
$$

where $\sqsubseteq$ permits replacement of subtrees by bottom and identifies bound names. To justify this syntactically, replacement of subterms by bottom commutes monotonically with substitution. A contraction in a partially erased term can be lifted to the corresponding contraction in the original term; if an erased function-head prevents matching a contraction, its result is bottom and is still below the original subtree. Induction over a finite reduction sequence therefore exhibits the erasure of $N^J$ as a partial reduct of a beta-equivalent version of $M$. Bottom contractions only prune this partial tree. Ordinary beta contractions alone preserve the [Böhm tree](../../../../../bohm-tree.md); the extra pruning explains why semantic inclusion here has the opposite orientation to the tree comparison.

Let $\mathcal A(M)$ be the [finite Böhm approximants](../../../../../finite-bohm-approximant.md) of $M$. Their grammar is

$$
A::=\bot\ \mid\ \lambda x_1\cdots x_n.yA_1\cdots A_r.
$$

Equivalently, they are finite beta-bottom normal forms obtained from a term beta-equivalent to $M$ by replacing subterms by bottom. The [approximation theorem for the graph model](../../../../../approximation-theorem-for-the-graph-model.md) is

$$
\boxed{\llbracket M\rrbracket_\rho=\bigcup_{A\in\mathcal A(M)}\llbracket A\rrbracket_\rho.}
$$

Here is a full proof. First, every indexed interpretation lies below the unindexed one. Increasing any occurrence index can only increase it, so the indexed interpretations form a directed family. Their union is the unindexed interpretation:

$$
\llbracket M\rrbracket_\rho=\bigcup_I\llbracket M^I\rrbracket_\rho.
$$

Prove this by [structural induction](../../../../../structural-induction.md). It is immediate for variables and bottom. At application, membership of an output has one finite-input witness in the graph; structural induction captures its graph entry and the finitely many required argument entries at finite child indices, and a root index at least the output captures it. At abstraction, a graph entry $\langle k,t\rangle$ is determined by one body membership in the finite-input environment $\rho[x:=e_k]$; structural induction captures that membership at finite body indices, and a root index at least $\langle k,t\rangle$ captures the entry. This proves both inclusions in the union identity without assuming the approximation theorem.

Now fix $I$ and reduce the fully indexed term to its normal form $A^J$, using the permitted normalization hypothesis. Its erasure $A$ has neither a beta redex nor a bottom-headed abstraction/application, so has the displayed approximant grammar. The lifting and pruning argument above gives $A\in\mathcal A(M)$. The semantic inequality along its finite reduction sequence gives

$$
\llbracket M^I\rrbracket_\rho\subseteq\llbracket A^J\rrbracket_\rho\subseteq\llbracket A\rrbracket_\rho.
$$

Taking the union over $I$ proves inclusion of the left side of the approximation theorem in the right. For the reverse inclusion, choose $A\in\mathcal A(M)$ and a beta-equivalent term from which it is obtained by erasing subterms. Beta soundness gives that term the same interpretation as $M$; erasure replaces interpretations by the least element, and every semantic constructor is monotone. Thus $\llbracket A\rrbracket_\rho\subseteq\llbracket M\rrbracket_\rho$. Taking the union finishes the proof. In particular an [unsolvable lambda term](../../../../../unsolvable-lambda-term.md) has only the bottom approximant and therefore has empty interpretation in $P\omega$.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
