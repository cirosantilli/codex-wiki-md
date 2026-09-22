<h1 id="6c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $x(t)=1+u(t)$. Retaining terms linear in $u$ gives

$$
u'(t)=\alpha\bigl[u(t)-2u(t-T)\bigr].
$$

The exponential ansatz $u=e^{\lambda t}$ gives the [characteristic equation of a delay differential equation](../../../../../../characteristic-equation-of-a-delay-differential-equation.md)

$$
\lambda=\alpha\left(1-2e^{-\lambda T}\right).
$$

At $T=0$ its root is $\lambda=-\alpha$, and the remaining delay roots lie far in the left half-plane, so the equilibrium is stable for sufficiently small $T$.

A stability change can first occur when $\lambda=i\omega$. Separating real and imaginary parts gives

$$
\cos(\omega T)=\frac12,
\qquad
\omega=2\alpha\sin(\omega T).
$$

For the first positive crossing, $\omega T=\pi/3$ and $\omega=\sqrt3\alpha$. Thus

$$
\boxed{T_c=\frac{\pi}{3\sqrt3\alpha}.}
$$

All positive-frequency crossings have $\omega T=\pi/3+2\pi k$, so there is no earlier imaginary-axis crossing. Implicit differentiation of

$$
F(\lambda,T)=\lambda-\alpha+2\alpha e^{-\lambda T}=0
$$

gives, with $q=\alpha T_c$,

$$
\operatorname{Re}\frac{d\lambda}{dT}
=\frac{3\alpha^2}{(1-q)^2+3q^2}>0,
$$

so the conjugate pair crosses into the right half-plane as $T$ increases. Therefore the [stability threshold for delayed quadratic crowding](../../../../../../stability-threshold-for-delayed-quadratic-crowding.md) is

$$
\boxed{x=1\text{ is stable for }0\leq T<T_c\text{ and loses stability at }T=T_c.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6C](../../6c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
