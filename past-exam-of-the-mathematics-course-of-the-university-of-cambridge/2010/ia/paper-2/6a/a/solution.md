<h1 id="6a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substitute the [power series](../../../../../../power-series.md) and compare coefficients. The constant coefficient gives $-a_1-a_0=0$. For $k\geq1$, the coefficient of $x^k$ gives

$$
(k+1)(k-1)a_{k+1}+(k-1)a_k=0.
$$

Thus $a_1=-a_0$, while the $k=1$ equation places no restriction on $a_2$. For $k\geq2$,

$$
a_{k+1}=-\frac{a_k}{k+1},\qquad
a_k=\frac{2a_2(-1)^k}{k!}.
$$

The [power series](../../../../../../power-series.md) therefore sums to

$$
y=a_0(1-x)+2a_2(e^{-x}-1+x).
$$

Renaming the two arbitrary constants gives **$\boxed{y(x)=C(1-x)+De^{-x}}$**.

Both functions solve the equation by direct substitution. Their [Wronskian](../../../../../../wronskian.md), in the order $1-x,e^{-x}$, is $xe^{-x}$, which is nonzero for $x\ne0$. Hence they give the full two-dimensional solution space on either interval away from the singular point. Both are entire, and the displayed formula also gives every twice continuously differentiable solution through zero: matching $y(0)$ and $y''(0)$ fixes the same $C,D$ on the two sides.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6A](../../6a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
