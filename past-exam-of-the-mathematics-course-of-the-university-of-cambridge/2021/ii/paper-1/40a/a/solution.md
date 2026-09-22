<h1 id="40a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [acoustic velocity potential](../../../../../../acoustic-velocity-potential.md) convention

$$
\mathbf u=\nabla\phi,
\qquad
\widetilde p=-\rho_0\frac{\partial\phi}{\partial t}.
$$

Put

$$
k=\frac{\omega}{c_0},
\qquad
\alpha=kR.
$$

For a spherically symmetric harmonic solution, write

$$
\phi(r,t)=F(r)\sin\omega t.
$$

The wave equation and

$$
\nabla^2F=\frac1r\frac{d^2}{dr^2}(rF)
$$

give the radial Helmholtz equation

$$
\frac{d^2}{dr^2}(rF)+k^2(rF)=0.
$$

The rigid inner sphere requires

$$
u_r(R,t)=F'(R)\sin\omega t=0.
$$

A form satisfying this condition automatically is

$$
F(r)=\frac C r
\left[
\cos k(r-R)+\frac1{kR}\sin k(r-R)
\right].
$$

Indeed, if the bracket is $h(r)$, then $h(R)=1$ and $h'(R)=1/R$, so $(h/r)'=0$ at $R$.

At the outer sphere,

$$
\varepsilon p_0\cos\omega t
=-\rho_0\omega F(2R)\cos\omega t,
$$

so

$$
F(2R)=-\frac{\varepsilon p_0}{\rho_0\omega}.
$$

Since

$$
F(2R)=\frac C{2R}
\left(\cos\alpha+\frac{\sin\alpha}{\alpha}\right),
$$

we obtain

$$
C=-\frac{2R\varepsilon p_0}
{\rho_0\omega(\cos\alpha+\alpha^{-1}\sin\alpha)}.
$$

Therefore

$$
\boxed{
\phi(r,t)
=-\frac{2R\varepsilon p_0}{\rho_0\omega r}
\frac{\cos k(r-R)+(kR)^{-1}\sin k(r-R)}
{\cos\alpha+\alpha^{-1}\sin\alpha}
\sin\omega t}.
$$

The assumption $\alpha\leq\pi/2$ keeps the displayed denominator positive.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40A](../../40a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
