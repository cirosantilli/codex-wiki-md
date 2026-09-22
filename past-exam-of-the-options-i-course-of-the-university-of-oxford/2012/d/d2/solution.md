<h1 id="d/d2/solution">Solution</h1>

↑ **Parent:** [D2](../d2.md)

On any bounded parameter interval $|t|\leq T$, the [derivative](../../../../derivative.md) of the integrand has the integrable majorant

$$
\left|\frac\partial{\partial t}\bigl[e^{-x^2}\cos(2xt^2)\bigr]\right|
=|4xt e^{-x^2}\sin(2xt^2)|\leq4Tx e^{-x^2}.
$$

The [dominated convergence theorem](../../../../dominated-convergence-theorem.md) therefore justifies [differentiation under the integral sign](../../../../differentiation-under-the-integral-sign.md) at every real $t$, giving

$$
f'(t)=-4t\int_0^\infty xe^{-x^2}\sin(2xt^2)\,dx.
$$

Use [integration by parts](../../../../integration-by-parts.md) in this absolutely convergent integral, with $xe^{-x^2}\,dx=-\tfrac12d(e^{-x^2})$. Both boundary terms vanish, since the sine is zero at $x=0$ and the Gaussian tends to zero at infinity. Hence

$$
\int_0^\infty xe^{-x^2}\sin(2xt^2)\,dx
=t^2\int_0^\infty e^{-x^2}\cos(2xt^2)\,dx=t^2f(t).
$$

It follows that $f'=-4t^3f$, or equivalently $(e^{t^4}f(t))'=0$. This identity holds on all of $\mathbb R$, including zero. With the supplied Gaussian integral value,

$$
\boxed{f(t)=\frac{\sqrt\pi}{2}e^{-t^4}\qquad(t\in\mathbb R).}
$$

The fourth power comes from the printed phase $2xt^2$; the parameter has been differentiated with that phase throughout.

## ↑ Ancestors (12)

1. [D2](../d2.md)
2. [D](../../d.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
