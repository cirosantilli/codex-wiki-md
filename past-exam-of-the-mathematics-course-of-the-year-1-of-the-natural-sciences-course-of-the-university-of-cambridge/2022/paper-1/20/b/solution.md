<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First suppose $\alpha>0$. [Differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md), justified on compact positive parameter [intervals](../../../../../interval-mathematics.md) by an integrable bound, gives

$$
f'(\alpha)=\int_0^\infty\frac{\ln(\alpha^2+x^2)}{1+x^2}\,dx+2\alpha^2\int_0^\infty\frac{dx}{(x^2+\alpha^2)(x^2+1)}.
$$

The first [integral](../../../../../integral-split.md) is $f(\alpha)/\alpha$. For $\alpha\ne1$, use the [partial fraction decomposition](../../../../../partial-fraction-decomposition.md)

$$
\frac1{(x^2+\alpha^2)(x^2+1)}=\frac1{1-\alpha^2}\left(\frac1{x^2+\alpha^2}-\frac1{x^2+1}\right).
$$

The standard [inverse tangent](../../../../../inverse-tangent.md) [antiderivatives](../../../../../antiderivative.md) then give

$$
\int_0^\infty\frac{dx}{(x^2+\alpha^2)(x^2+1)}=\frac1{1-\alpha^2}\left(\frac\pi{2\alpha}-\frac\pi2\right)=\frac\pi{2\alpha(1+\alpha)}.
$$

The same value holds at $\alpha=1$ by [continuity](../../../../../continuous-function.md), or by direct [integration](../../../../../integral-split.md). Hence the proposed [first-order linear differential equation](../../../../../first-order-linear-differential-equation.md) is valid on the positive parameter range:

$$
\boxed{f'(\alpha)-\frac{f(\alpha)}\alpha=\frac{\pi\alpha}{1+\alpha},\qquad\alpha>0.}
$$

Divide by $\alpha$ to recognise a [quotient rule](../../../../../quotient-rule.md) derivative:

$$
\left(\frac{f(\alpha)}\alpha\right)'=\frac\pi{1+\alpha},\qquad f(\alpha)=\alpha[\pi\ln(1+\alpha)+C].
$$

To fix $C$, the value $f(0)=0$ alone is insufficient, since every displayed solution tends to zero there. Instead consider

$$
\lim_{\alpha\to0^+}\frac{f(\alpha)}\alpha=\int_0^\infty\frac{\ln(x^2)}{1+x^2}\,dx.
$$

This limit follows from the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md): for $0<\alpha\leq1$ and $0<x<1$, the logarithm's [absolute value](../../../../../absolute-value.md) is bounded by $2|\ln x|+\ln2$; for $x\geq1$, it is at most $\ln(1+x^2)$. After division by $1+x^2$, these are integrable. The limiting [improper integral](../../../../../improper-integral.md) is absolutely convergent, and the [substitution rule](../../../../../integration-by-substitution.md) $x=1/t$ changes it into its own negative. Its value is therefore zero, giving $C=0$. Thus

$$
\boxed{\int_0^\infty\frac{\alpha\ln(\alpha^2+x^2)}{1+x^2}\,dx=\pi\alpha\ln(1+\alpha),\qquad\alpha>0.}
$$

The question calls $\alpha$ a real parameter, but this last formula and the proposed differential equation do not hold on the entire real axis. The defining [integral](../../../../../integral-split.md) is odd in $\alpha$, because its logarithm depends on $\alpha^2$. Applying the positive-parameter result to $|\alpha|$ therefore gives the correct extension

$$
\boxed{f(\alpha)=\pi\alpha\ln(1+|\alpha|),\qquad\alpha\in\mathbb R,}
$$

with $f(0)=0$. In particular, for $\alpha<0$, the right-hand side of the differential equation must be $-\pi\alpha/(1-\alpha)$; for every $\alpha\ne0$ the unified expression is $\pi|\alpha|/(1+|\alpha|)$. The [logarithmic quadratic parameter integral](../../../../../logarithmic-quadratic-parameter-integral.md) therefore provides the requested identity on its valid range and the corrected answer elsewhere.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
