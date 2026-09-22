<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiply the [Sturm-Liouville form](../../../../../sturm-liouville-form.md) for $y_n$ by $y_m$ and subtract the equation for $y_m$ multiplied by $y_n$. Integration gives

$$
(n^2-m^2)\int_{-1}^1w\,y_ny_m\,dx
=\left[p(y_ny_m'-y_my_n')\right]_{-1}^1=0.
$$

The boundary expression is zero because $p\to0$ and the functions and first [derivatives](../../../../../derivative.md) remain finite. Since $n,m$ are distinct positive integers, this proves

$$
\boxed{\int_{-1}^1y_ny_m\sqrt{1-x^2}\,dx=0.}
$$

For the [derivatives](../../../../../derivative.md), apply [integration by parts](../../../../../integration-by-parts.md) once to the same [Sturm-Liouville form](../../../../../sturm-liouville-form.md):

$$
\int_{-1}^1p\,y_n'y_m'\,dx
=\left[py_n'y_m\right]_{-1}^1-\int_{-1}^1(py_n')'y_m\,dx
=(n^2-1)\int_{-1}^1w\,y_ny_m\,dx=0.
$$

Thus the new weight is

$$
\boxed{w_1(x)=(1-x^2)^{3/2}.}
$$

This is [derivative orthogonality when the Sturm-Liouville potential vanishes](../../../../../derivative-orthogonality-when-the-sturm-liouville-potential-vanishes.md). For $n=1$ the [derivative](../../../../../derivative.md) is identically zero, which is consistent with the identity.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
