<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Seek a positive weight such that the [differential operator](../../../../../differential-operator.md) becomes $-w^{-1}(py')'$. Matching the second [derivative](../../../../../derivative.md) gives $p=w(1-x^2)$, while matching the first [derivative](../../../../../derivative.md) requires $p'=-xw$. Consequently

$$
(1-x^2)w'-2xw=-xw,\qquad \frac{w'}w=\frac{x}{1-x^2}.
$$

Choosing the multiplicative constant to be one gives

$$
\boxed{w(x)=\frac1{\sqrt{1-x^2}},\qquad p(x)=\sqrt{1-x^2},\qquad -(py_n')'=n^2wy_n}.
$$

This is [Sturm-Liouville form](../../../../../sturm-liouville-form.md) with zero potential term. Multiply the equations for $y_n,y_m$ by $y_m,y_n$, subtract, and integrate. The [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md) gives

$$
(n^2-m^2)\int_{-1}^1wy_ny_m\,dx
=\left[p(y_ny_m'-y_my_n')\right]_{-1}^{1}=0.
$$

The boundary expression vanishes because $p\to0$ and the functions and their [derivatives](../../../../../derivative.md) are finite. Since $n,m\geq0$ are distinct, their [eigenvalues](../../../../../eigenvalue.md) $n^2,m^2$ are distinct, proving

$$
\boxed{\int_{-1}^{1}\frac{y_n(x)y_m(x)}{\sqrt{1-x^2}}\,dx=0\quad(n\ne m)}.
$$

The endpoint singularities of the weight are integrable, so these [weighted inner products](../../../../../weighted-inner-product.md) exist.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
