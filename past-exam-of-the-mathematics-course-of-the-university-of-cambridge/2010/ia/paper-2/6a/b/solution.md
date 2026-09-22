<h1 id="6a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For two solutions $y_1,y_2$, define their [Wronskian](../../../../../../wronskian.md) by

$$
W=y_1y_2'-y_1'y_2.
$$

Differentiation and substitution of the [second-order linear differential equation](../../../../../../second-order-linear-differential-equation.md) give

$$
W'=y_1y_2''-y_1''y_2
=y_1(-py_2'-qy_2)-(-py_1'-qy_1)y_2=-pW.
$$

This proves the [Abel identity](../../../../../../abel-s-identity.md) and hence

$$
\boxed{W(x)=C\exp\left(-\int_{x_0}^x p(r)\,dr\right).}
$$

On an interval where the known solution $y_1$ does not vanish,

$$
\left(\frac{y_2}{y_1}\right)'=\frac{W}{y_1^2}.
$$

Integrating gives the [reduction of order](../../../../../../reduction-of-order.md) formula

$$
\boxed{y_2(x)=y_1(x)\int_{x_0}^x
\frac{\exp(-\int_{x_0}^s p(r)\,dr)}{y_1(s)^2}\,ds.}
$$

Choosing the normalization $C=1$ makes the [Wronskian](../../../../../../wronskian.md) nonzero, so this solution is linearly independent of $y_1$. To verify it really solves the equation, write $y_2=y_1h$. Its equation reduces to

$$
y_1h''+(2y_1'+py_1)h'=0;
$$

the integrand gives $h'=\exp(-\int p)/y_1^2$, which satisfies this equation on differentiation. Adding an integration constant only adds a multiple of $y_1$. The formula is local where $y_1\ne0$; at a zero of $y_1$ with regular coefficients, the actual solution can be continued by initial-value existence and uniqueness, even if its integral representation has an apparent singularity.

## ↑ Ancestors (11)

1. [B](../b.md)
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
