<h1 id="33c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Korteweg-De Vries equation](../../../../../../korteweg-de-vries-equation.md) is the compatibility condition $L_t=[P,L]$ for the [Lax pair](../../../../../../lax-pair.md)

$$
L=-\partial_x^2+u,
\qquad
P=-4\partial_x^3+6u\partial_x+3u_x.
$$

For rapidly decaying initial data, first solve the direct [KdV Schrodinger spectral problem](../../../../../../kdv-schrodinger-spectral-problem.md)

$$
L\psi=k^2\psi.
$$

Comparing its [Jost solutions](../../../../../../jost-solution.md) at the two spatial infinities produces the [KdV scattering data](../../../../../../kdv-scattering-data.md): the reflection coefficient $R(k)$ on the continuous spectrum, discrete eigenvalues $-\kappa_n^2$, and norming amplitudes $c_n$ for the bound states.

The Lax evolution is isospectral. More precisely, the [Time evolution of KdV scattering data](../../../../../../time-evolution-of-kdv-scattering-data.md) is

$$
\kappa_n(t)=\kappa_n(0),\qquad
R(k,t)=R(k,0)e^{8ik^3t},\qquad
c_n(t)=c_n(0)e^{4\kappa_n^3t}.
$$

This is the simple linear evolution that makes the nonlinear initial-value problem tractable.

To invert the data, form

$$
F(s,t)
=\frac1{2\pi}\int_{-\infty}^{\infty}
R(k,t)e^{iks}\,dk
+\sum_n c_n(t)^2e^{-\kappa_ns}.
$$

Solve the [Gelfand-Levitan-Marchenko equation](../../../../../../marchenko-equation.md)

$$
K(x,y;t)+F(x+y,t)
+\int_x^\infty K(x,z;t)F(z+y,t)\,dz=0,
\qquad y\geq x,
$$

and reconstruct

$$
\boxed{u(x,t)=-2\frac{\partial}{\partial x}K(x,x;t)}.
$$

Direct scattering at $t=0$, linear evolution of the data, and this inverse step constitute the [inverse scattering transform](../../../../../../inverse-scattering-transform.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [33C](../../33c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
