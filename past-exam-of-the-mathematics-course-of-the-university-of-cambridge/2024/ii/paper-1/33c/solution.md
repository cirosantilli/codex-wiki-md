<h1 id="33c/solution">Solution</h1>

↑ **Parent:** [33C](../33c.md)

Differentiate the spatial equation with respect to $t$ and the temporal equation with respect to $x$. Substitution of

$$
\psi_x=ik\psi+u,
\qquad
\psi_t=-ik^2\psi+iu_x-ku
$$

into $\psi_{xt}-ik\psi_t$ cancels every term involving $\psi$, $u$, and $u_x$, leaving

$$
\psi_{xt}-ik\psi_t=iu_{xx}.
$$

The left side is $u_t$ by differentiating $\psi_x-ik\psi=u$, so consistency is exactly $u_t=iu_{xx}$. This is a [scalar](../../../../../scalar.md) [Lax pair](../../../../../lax-pair.md) formulation.

Taking the half-line Fourier transform and integrating twice by parts gives

$$
\partial_t\widehat u(k,t)+ik^2\widehat u(k,t)
=kh(t)-iu_x(0,t).
$$

Multiplication by $e^{ik^2t}$ and integration in time yields

$$
\boxed{
\widehat u(k,t)e^{ik^2t}-\widehat u_0(k)
=\int_0^t e^{ik^2\tau}
 [kh(\tau)-iu_x(0,\tau)]\,d\tau.}
$$

Replace $k$ by $-k$ and subtract. The unknown Neumann boundary value cancels:

$$
e^{ik^2t}\bigl[\widehat u(k,t)-\widehat u(-k,t)\bigr]
=\widehat u_0(k)-\widehat u_0(-k)
 +2k\int_0^t e^{ik^2\tau}h(\tau)\,d\tau.
$$

For $x>0$, Fourier inversion of the zero extension gives

$$
\int_{\mathbb R}e^{ikx}\widehat u(-k,t)\,dk=0.
$$

Inverting the preceding identity therefore gives

$$
\begin{aligned}
u(x,t)
={}&\frac1{2\pi}\int_{-\infty}^{\infty}
 e^{-ik^2t+ikx}[\widehat u_0(k)-\widehat u_0(-k)]\,dk\\
&+\frac1\pi\int_{-\infty}^{\infty}\int_0^t
 e^{-ik^2(t-\tau)+ikx}\,k h(\tau)\,d\tau\,dk.
\end{aligned}
$$

Thus

$$
\boxed{G(k,\tau)=k h(\tau).}
$$

This elimination is the [global relation for the half-line free Schrodinger equation](../../../../../global-relation-for-the-half-line-free-schrodinger-equation.md).

## ↑ Ancestors (10)

1. [33C](../33c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
