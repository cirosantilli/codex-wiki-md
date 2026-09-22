# Power-set product cardinality inequality

↑ **Parent:** [Power set](power-set.md)

For arbitrary [sets](set-split.md) $A,B$ each containing at least two elements, the displayed inequality follows by explicitly encoding two [subsets](subset.md) in disjoint parts of a [Cartesian product](cartesian-product.md). Choose $a_0\ne a_1$ and $b_0\ne b_1$, put $S$ along the row $A\times\{b_0\}$, put $T\setminus\{b_0\}$ along the column $\{a_0\}\times(B\setminus\{b_0\})$, and add the extra point $(a_1,b_1)$ precisely when $b_0\in T$. These regions are disjoint, so the encoding recovers both $S$ and $T$ and is an [injection](injective-function.md) from $\mathcal P(A)\times\mathcal P(B)$ into $\mathcal P(A\times B)$. This proves the [cardinality](cardinality.md) inequality even for infinite [sets](set-split.md). For finite sizes $a,b\geq2$, the same result is $2^{ab}\geq2^{a+b}$, since $ab-a-b=(a-1)(b-1)-1\geq0$. Mapping $(S,T)$ to $S\times T$ is insufficient because all pairs with an empty factor collapse.

## ↑ Ancestors (7)

1. [Power set](power-set.md)
2. [Set](set-split.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/1/d/ii/solution.md)
