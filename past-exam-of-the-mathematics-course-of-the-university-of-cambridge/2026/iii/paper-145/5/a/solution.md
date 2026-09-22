<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Alon-Tarsi lemma](../../../../../../alon-tarsi-lemma.md) says that if $\deg f\leq d_1+\cdots+d_n$ and $A_i$ consists of $d_i+1$ distinct field elements, then

$$
[x_1^{d_1}\cdots x_n^{d_n}]f
=\sum_{a_i\in A_i}
\frac{f(a_1,\ldots,a_n)}
{\prod_i\prod_{b\in A_i\setminus\{a_i\}}(a_i-b)}.
$$

This follows by applying univariate Lagrange interpolation successively in each variable.

If the displayed coefficient is nonzero, at least one summand has $f(a_1,\ldots,a_n)\ne0$. This is the coefficient form of the [Combinatorial Nullstellensatz](../../../../../../combinatorial-nullstellensatz.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 145](../../../paper-145-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
