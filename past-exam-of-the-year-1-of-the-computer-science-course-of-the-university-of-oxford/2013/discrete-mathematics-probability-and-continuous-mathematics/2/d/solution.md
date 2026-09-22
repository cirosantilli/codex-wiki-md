<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First consider powers of four, with a fixed finite base value. For a [mathematical induction](../../../../../mathematical-induction.md) hypothesis $x_{n/4}\leq C(n/4)^2$, the [recurrence relation](../../../../../recurrence-relation.md) gives

$$
x_n\leq4C(n/4)^2+n^2=(C/4+1)n^2\leq Cn^2
$$

provided $C\geq4/3$ and $C$ also covers the base value.

The allowed integer rounding needs a little more care. Suppose the [recurrence relation](../../../../../recurrence-relation.md) is applied above fixed base cases, as usual; applying $x_1=4x_1+1$ with a ceiling would not define a positive sequence. For either rounding write $m=\lceil n/4\rceil$ or $m=\lfloor n/4\rfloor$. For $n\geq6$,

$$
m\leq\frac{n+3}{4},\qquad\frac{4m^2}{n^2}\leq\frac14\left(1+\frac3n\right)^2\leq\frac9{16},\qquad m<n.
$$

Choose $C\geq16/7$ large enough to bound all finitely many positive-index base values below $6$. By [strong induction](../../../../../strong-induction.md),

$$
x_n=4x_m+n^2\leq4Cm^2+n^2\leq(9C/16+1)n^2\leq Cn^2.
$$

This argument starts at $n=6$, so the floor convention's index zero, if used in an earlier base calculation, is absorbed into those fixed initial values. Thus, for either convention with a well-defined finite base,

$$
\boxed{x_n=O(n^2).}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
