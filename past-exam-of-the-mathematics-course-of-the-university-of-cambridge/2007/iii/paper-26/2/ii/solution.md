<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose a nonempty set $S$ had no minimal member for the [intersection-power-set predecessor relation](../../../../../../intersection-power-set-predecessor-relation.md). Put $b=\bigcap S$, which is a set by [separation](../../../../../../axiom-schema-of-specification.md). For every $y\in S$ there is an $x\in S$ with $\mathcal P(x\cap y)\subseteq y$. Since $b\subseteq x\cap y$, this gives $\mathcal P(b)\subseteq y$. Intersecting over every $y\in S$ yields $\mathcal P(b)\subseteq b$.

Now form the diagonal subset $d=\{u\in b:u\notin u\}$. It belongs to $\mathcal P(b)$, hence to $b$, so its defining condition implies $d\in d\iff d\notin d$, a contradiction. Thus $\boxed{R\text{ is well-founded}.}$ This is a [Cantor diagonal argument](../../../../../../cantor-diagonal-argument.md); it uses neither the [Axiom of foundation](../../../../../../axiom-of-regularity.md) nor the [axiom of choice](../../../../../../axiom-of-choice.md). In particular, no selection of an infinite descending sequence is needed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
