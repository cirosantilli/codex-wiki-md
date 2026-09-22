<h1 id="16d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write

$$
\frac1{|\mathbf x-\mathbf y|}
=\frac1{|\mathbf x|}
\left(1-2\frac{\mathbf x\mathbin{\cdot}\mathbf y}{|\mathbf x|^2}
+\frac{|\mathbf y|^2}{|\mathbf x|^2}\right)^{-1/2}.
$$

Using the [Taylor series](../../../../../../taylor-series.md)

$$
(1+s)^{-1/2}=1-\frac12s+\frac38s^2+O(s^3)
$$

and retaining terms through second order in $|\mathbf y|/|\mathbf x|$ gives

$$
\boxed{
\frac1{|\mathbf x-\mathbf y|}
=\frac1{|\mathbf x|}
\left[
1+\frac{\mathbf x\mathbin{\cdot}\mathbf y}{|\mathbf x|^2}
+\frac{3(\mathbf x\mathbin{\cdot}\mathbf y)^2-|\mathbf x|^2|\mathbf y|^2}
{2|\mathbf x|^4}
+O\!\left(\frac{|\mathbf y|^3}{|\mathbf x|^3}\right)
\right]}.
$$

This is the beginning of the [multipole expansion](../../../../../../electric-multipole-expansion.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16D](../../16d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
