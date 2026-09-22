<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce a constant [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\mu$ for this [isoperimetric constraint](../../../../../isoperimetric-constraint.md) and make $A-\mu(C-B)$ stationary. Its integrand is $(1-\mu)y-\mu y'^2$, so the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) gives

$$
1-\mu+2\mu y''=0.
$$

The endpoint conditions therefore force a parabola $y=Kx(1-x)$. Its area and budget are

$$
A=\frac K6,\qquad C=\frac K6+\frac{K^2}{3}=B.
$$

Solving the quadratic and choosing positive area gives

$$
\boxed{K=\frac{\sqrt{1+48B}-1}{4},\qquad y_{\mathrm{opt}}(x)=\frac{\sqrt{1+48B}-1}{4}x(1-x),\qquad A_{\max}=\frac{\sqrt{1+48B}-1}{24}.}
$$

This requires $B>0$; no positive-area barrier is possible for a nonpositive budget. The corresponding multiplier is $\mu=1/(1+4K)>0$.

To verify a global maximum rather than just stationarity, use the [sharp area-cost bound for a barrier with fixed endpoints](../../../../../sharp-area-cost-bound-for-a-barrier-with-fixed-endpoints.md). For $w=x(1-x)$, [integration by parts](../../../../../integration-by-parts.md) gives $2A=\int_0^1y'w'dx$, and $\int_0^1w'^2dx=1/3$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) implies

$$
\int_0^1y'^2dx\geq12A^2,\qquad B\geq A+12A^2.
$$

For $A>0$ the last expression increases strictly, yielding exactly the boxed upper bound. Equality requires $y'$ proportional to $w'$, hence $y=Kw$ after imposing the endpoints. Thus the displayed optimum is unique and lies above the baseline throughout the interior.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
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
