<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

Separation $y=T(t)X(x)$ and the fixed-end conditions give

$$
X_n(x)=\sin(n\pi x),
\qquad
T_n''+T_n'+n^2\pi^2T_n=0.
$$

Put

$$
\omega_n=\sqrt{n^2\pi^2-\frac14}.
$$

The initial displacement and zero initial [velocity](../../../../../velocity.md) then give the [separated solution of the damped string equation](../../../../../separated-solution-of-the-damped-string-equation.md)

$$
\boxed{
y(t,x)=\sum_{n=1}^{\infty}a_ne^{-t/2}
\left(
\cos(\omega_nt)+\frac{\sin(\omega_nt)}{2\omega_n}
\right)\sin(n\pi x)}.
$$

For the triangular initial displacement,

$$
\begin{aligned}
a_n
&=2\int_0^1y(0,x)\sin(n\pi x)\,dx\\
&=\boxed{\frac{4\sin(n\pi/2)}{n^2\pi^2}}.
\end{aligned}
$$

Thus the even coefficients vanish and the odd ones alternate in sign.

Let

$$
T_n(t)=a_ne^{-t/2}
\left(\cos(\omega_nt)+\frac{\sin(\omega_nt)}{2\omega_n}\right).
$$

Then

$$
T_n'(t)=-a_ne^{-t/2}
\frac{n^2\pi^2}{\omega_n}\sin(\omega_nt).
$$

Orthogonality of the sine and cosine modes, equivalently the [Parseval identity](../../../../../parseval-identity.md), gives

$$
\boxed{
E(t)=\frac14\sum_{n=1}^{\infty}a_n^2e^{-t}
\left[
\frac{n^4\pi^4}{\omega_n^2}\sin^2(\omega_nt)
+n^2\pi^2
\left(\cos(\omega_nt)+
\frac{\sin(\omega_nt)}{2\omega_n}\right)^2
\right]}.
$$

The sign of its [derivative](../../../../../derivative.md) is clearest directly from the equation. Integration by parts, using $y_t=0$ at the fixed endpoints, yields

$$
\begin{aligned}
E'(t)
&=\int_0^1(y_ty_{tt}+y_xy_{xt})\,dx\\
&=\int_0^1y_t(y_{tt}-y_{xx})\,dx
=-\int_0^1y_t^2\,dx\leq0.
\end{aligned}
$$

This is the [energy dissipation identity for a linearly damped string](../../../../../energy-dissipation-identity-for-a-linearly-damped-string.md).

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
