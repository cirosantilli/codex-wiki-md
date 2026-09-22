<h1 id="14b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Insert

$$
w(z)=\int_\gamma e^{zt}f(t)\,dt
$$

into the equation. Since $w'=\int_\gamma te^{zt}f\,dt$ and $w''=\int_\gamma t^2e^{zt}f\,dt$, use $ze^{zt}=\partial_te^{zt}$ and [integration by parts](../../../../../../integration-by-parts.md):

$$
zw''+2aw'+zw
=\left[e^{zt}(1+t^2)f(t)\right]_{\partial\gamma}
+\int_\gamma e^{zt}
\left[
2atf-\frac d{dt}\bigl((1+t^2)f\bigr)
\right]dt.
$$

The integral vanishes when

$$
(1+t^2)f'=2(a-1)tf,
$$

so, up to a constant and on a consistently chosen branch,

$$
\boxed{\ f(t)=(1+t^2)^{a-1}\ }.
$$

The remaining contour condition is

$$
\boxed{\
\left[e^{zt}(1+t^2)^a\right]_{\partial\gamma}=0\
}.
$$

This is the [Laplace contour-integral method for a linear differential equation](../../../../../../laplace-contour-integral-method-for-a-linear-differential-equation.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14B](../../14b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
