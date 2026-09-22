<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $S:\mathbb R^p\rightrightarrows\mathbb R^q$ be a [set-valued mapping](../../../../../../set-valued-mapping.md) and let $\bar v\in S(\bar u)$. The [Aubin property](../../../../../../aubin-property.md) at $(\bar u,\bar v)$ means there are neighborhoods $U$ of $\bar u$, $V$ of $\bar v$, and a finite constant $\kappa\geq0$ such that

$$
\boxed{S(u)\cap V\subset S(u')+\kappa\|u-u'\|_2\mathbb B_q
\quad\text{for every }u,u'\in U}.
$$

Here $\mathbb B_q$ is the closed unit ball. Equivalently, every solution $v\in S(u)$ near $\bar v$ can be matched to a solution $v'\in S(u')$ within $\kappa\|u-u'\|_2$. The localization is on the left-hand side: the matching point need not be in $V$. The property is also called the [Lipschitz-like property](../../../../../../aubin-property.md).

For [sensitivity analysis](../../../../../../sensitivity-analysis.md), let $u$ represent data or perturbations and $S(u)$ the set of feasible or optimal solutions. The [Aubin property](../../../../../../aubin-property.md) bounds how far a nearby solution can move when the data change. Taking $u=\bar u$, $v=\bar v$ also guarantees a nearby solution for each sufficiently small perturbation $u'$. It is a stability estimate for a relation, and by itself does not imply uniqueness or differentiability. For a single-valued solution map, it reduces to local [Lipschitz continuity](../../../../../../lipschitz-continuity.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
