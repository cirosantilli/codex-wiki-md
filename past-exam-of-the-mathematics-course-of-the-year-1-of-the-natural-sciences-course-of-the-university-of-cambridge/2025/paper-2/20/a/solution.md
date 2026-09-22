<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\Psi(\eta,\xi)=\psi(x,t)$. The inverse coordinate formulas $x=(\eta+\xi)/2$ and $t=(\eta-\xi)/(2c)$ are valid because $c>0$. The [multivariable chain rule](../../../../../multivariable-chain-rule.md) gives

$$
\partial_x=\partial_\eta+\partial_\xi,\qquad
\partial_t=c\partial_\eta-c\partial_\xi.
$$

Applying these operators twice and using the [symmetry of second derivatives](../../../../../symmetry-of-second-derivatives.md),

$$
\psi_{xx}=\Psi_{\eta\eta}+2\Psi_{\eta\xi}+\Psi_{\xi\xi},
\qquad
\frac1{c^2}\psi_{tt}=\Psi_{\eta\eta}-2\Psi_{\eta\xi}+\Psi_{\xi\xi}.
$$

Thus the [wave equation](../../../../../wave-equation-split.md) is equivalent to

$$
\boxed{\Psi_{\eta\xi}=0}.
$$

For each fixed $\eta$, the [partial derivative](../../../../../partial-derivative.md) $\Psi_\eta$ has zero [derivative](../../../../../derivative.md) with respect to $\xi$, so it is a [function](../../../../../function-split.md) of $\eta$ alone. Taking an [antiderivative](../../../../../antiderivative.md) in $\eta$ gives $\Psi=f(\eta)+g(\xi)$, where the integration constant may depend on $\xi$. Hence

$$
\boxed{\psi(x,t)=f(x+ct)+g(x-ct)}.
$$

Conversely, direct [partial differentiation](../../../../../partial-derivative.md) verifies the [wave equation](../../../../../wave-equation-split.md) for every twice [differentiable](../../../../../differentiable-function.md) pair $f,g$. The two terms describe profiles moving left and right respectively at [wave speed](../../../../../wave-speed.md) $c$ along the [characteristic lines for the one-dimensional wave equation](../../../../../characteristic-line-for-the-one-dimensional-wave-equation.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
