<h1 id="16i/solution">Solution</h1>

↑ **Parent:** [16I](../16i.md)

The [completeness theorem for propositional logic](../../../../../completeness-theorem-for-propositional-logic.md) states that for every set of formulae $\Gamma$ and formula $\varphi$,

$$
\boxed{\Gamma\models\varphi\quad\Longrightarrow\quad\Gamma\vdash\varphi}.
$$

With the [soundness theorem for propositional logic](../../../../../soundness-theorem-for-propositional-logic.md), this is an equivalence. It is also equivalent to saying that every [consistent set of formulae](../../../../../consistent-set-of-formulae.md) has a model.

The usual countable proof lists all formulae and extends a consistent theory one formula at a time. For an uncountable set of primitive propositions, use the [uncountable-language proof of propositional completeness](../../../../../uncountable-language-proof-of-propositional-completeness.md): order the consistent extensions of $\Gamma$ by inclusion. The union of every chain is consistent, since a proof of a contradiction would use only finitely many assumptions and hence would already lie in one member of the chain. [Zorn lemma](../../../../../zorn-s-lemma.md) gives a [maximal consistent set in propositional logic](../../../../../maximal-consistent-set-in-propositional-logic.md) $M$. Define a [Boolean valuation](../../../../../boolean-valuation.md) by $v(p)=1$ exactly when $p\in M$. The usual [structural induction](../../../../../structural-induction.md) on formulae proves the truth lemma

$$
v(\theta)=1\quad\Longleftrightarrow\quad\theta\in M,
$$

so $v$ is a model of $\Gamma$.

The [propositional compactness theorem](../../../../../propositional-compactness-theorem.md) says that a set $\Gamma$ is satisfiable if and only if every finite subset of $\Gamma$ is satisfiable. Only the forward implication is immediate. For the converse, if $\Gamma$ had no model, then $\Gamma\models\bot$, so completeness would give $\Gamma\vdash\bot$. Every [formal proof](../../../../../formal-proof.md) uses finitely many assumptions, so some finite $\Gamma_0\subseteq\Gamma$ would prove $\bot$ and, by soundness, would have no model, a contradiction.

The [decidability theorem for propositional logic](../../../../../decidability-theorem-for-propositional-logic.md) says that there is an algorithm deciding whether a propositional formula is a theorem. A formula contains only finitely many primitive propositions, even when the full language is uncountable. Its finite [truth table](../../../../../truth-table.md) decides whether it is valid, and completeness says that validity is equivalent to theoremhood.

Now let $(X,<)$ be the given [partially ordered set](../../../../../partially-ordered-set.md). For every distinct $x,y\in X$, introduce propositions $p_{xy}$ and $q_{xy}$. Form a propositional theory $T$ containing the following clauses:

- $p_{xy}\leftrightarrow\neg p_{yx}$ and $q_{xy}\leftrightarrow\neg q_{yx}$ for distinct $x,y$;
- $(p_{xy}\wedge p_{yz})\to p_{xz}$ and $(q_{xy}\wedge q_{yz})\to q_{xz}$ for pairwise distinct $x,y,z$;
- $p_{xy}$ and $q_{xy}$ whenever $x<y$ in the original order;
- $\neg(p_{xy}\wedge q_{xy})$ and $\neg(p_{yx}\wedge q_{yx})$ whenever $x$ and $y$ are incomparable in the original order.

The first two families say that $p$ and $q$ encode [strict total orders](../../../../../strict-total-order.md). The third makes both orders extend $<$, while the fourth makes them disagree on every incomparable pair.

Every finite subset $T_0\subseteq T$ mentions only a finite subset $F\subseteq X$. By hypothesis, the induced order on $F$ is a [two-dimensional poset](../../../../../two-dimensional-partially-ordered-set.md), so choose two total orders realizing it and assign the finitely many $p$ and $q$ variables accordingly. This satisfies $T_0$. Thus every finite subset of $T$ is satisfiable, and propositional compactness gives a model of all of $T$.

Define $x<_1y$ when $p_{xy}$ is true and $x<_2y$ when $q_{xy}$ is true. The clauses make $<_1$ and $<_2$ total orders on $X$. They both contain the original order, and their intersection contains no incomparable pair. Hence

$$
x<y\quad\Longleftrightarrow\quad x<_1y\text{ and }x<_2y,
$$

which proves the [finite-local characterization of two-dimensional partially ordered sets](../../../../../finite-local-characterization-of-two-dimensional-partially-ordered-sets.md).

## ↑ Ancestors (10)

1. [16I](../16i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
