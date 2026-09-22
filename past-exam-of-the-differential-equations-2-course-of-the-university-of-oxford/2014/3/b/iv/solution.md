<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $y(x)=Y(X)$ with $X=(1-x)/\sqrt\epsilon$. The transformed equation is

$$
Y''=Y-(1-\sqrt\epsilon X)^2+\epsilon(2+Y^2).
$$

Since the rescaled forcing contains $\sqrt\epsilon$, an [inner expansion](../../../../../inner-expansion.md) naturally uses powers of $\sqrt\epsilon$. Its leading term satisfies

$$
Y_0''=Y_0-1,\qquad Y_0(0)=0.
$$

The [asymptotic matching condition](../../../../../asymptotic-matching-condition.md) with the leading [outer solution](../../../../../outer-expansion.md) is

$$
Y_0(X)\longrightarrow y_0(1)=1\qquad(X\to\infty).
$$

The general solution is $Y_0=1+Ae^X+Be^{-X}$. Matching eliminates $Ae^X$, and the boundary condition gives $B=-1$. Hence

$$
\boxed{Y_0(X)=1-e^{-X},\qquad
y_{\rm inner}(x)\sim1-\exp\left(-\frac{1-x}{\sqrt\epsilon}\right).}
$$

This tends to the boundary value zero at $x=1$ and to the matching value one on the interior side of the layer. The negative sign in the exponential follows from measuring the [inner variable](../../../../../inner-variable.md) inward from the right endpoint.

For an optional uniform leading approximation, combine the leading inner and outer terms and subtract their common overlap value one. The [additive composite expansion](../../../../../additive-composite-expansion.md) is

$$
\boxed{y_{\rm comp}(x)=x^2-\exp\left(-\frac{1-x}{\sqrt\epsilon}\right).}
$$

It satisfies the right boundary condition exactly; its left-end discrepancy is the exponentially small value $-e^{-1/\sqrt\epsilon}$. The requested leading [inner expansion](../../../../../inner-expansion.md) is $Y_0$ above.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
