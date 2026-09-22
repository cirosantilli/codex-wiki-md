<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\lambda=\omega^2/g$ and

$$
Q=\frac{i\omega c}{2L}\big[(z+h)^2-(L-x)^2\big],\qquad G=f+Q.
$$

This polynomial is a [harmonic function](../../../../../harmonic-function.md): $Q_{xx}+Q_{zz}=0$. Also $Q_x(0,z)=i\omega c$, $Q_x(L,z)=0$ and $Q_z(x,-h)=0$. Thus $G$ satisfies [Laplace's equation](../../../../../laplace-equation.md) with homogeneous [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) on both side walls and the bottom. Its [Fourier cosine series](../../../../../fourier-cosine-series.md) consequently has the form

$$
\boxed{G(x,z)=\frac{a_0}{2}+\sum_{n=1}^{\infty}a_n\cos(k_nx)\cosh(k_n(z+h)),\qquad k_n=\frac{n\pi}{L}}.
$$

The surface condition becomes $G_z-\lambda G=H(x)$, where

$$
H(x)=\frac{i\omega c}{L}\left[h-\frac\lambda2\big(h^2-(L-x)^2\big)\right].
$$

For a nonzero forcing frequency away from the natural frequencies, the coefficients of the [oscillating-wall forcing of a rectangular tank](../../../../../oscillating-wall-forcing-of-a-rectangular-tank.md) are

$$
H_n=\frac2L\int_0^L H(x)\cos(k_nx)\,dx,\qquad a_0=-\frac{H_0}{\lambda},\qquad a_n=\frac{H_n}{k_n\sinh(k_nh)-\lambda\cosh(k_nh)}\quad(n\geq1).
$$

Here $k_0=0$ in the definition of $H_0$. In fact $H_n=2i\omega c\lambda/(Lk_n^2)$ for $n\geq1$, since $\int_0^L(L-x)^2\cos(k_nx)dx=2L/k_n^2$. The zero-mode coefficient ensures that the mean [surface elevation](../../../../../surface-elevation.md) is $hc/L$ in complex amplitude, exactly the first-order [volume conservation](../../../../../volume-conservation.md) adjustment to the moving wall.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the waves and compressible flow course of the University of Oxford](../../../../split.md)
6. [Waves and compressible flow course of the University of Oxford](../../../../../waves-and-compressible-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
