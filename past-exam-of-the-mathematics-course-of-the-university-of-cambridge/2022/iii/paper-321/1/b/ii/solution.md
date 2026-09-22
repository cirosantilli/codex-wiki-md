<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $P=K\rho^{1+1/n}$,

$$
c_s^2=\frac{dP}{d\rho}
=\frac{n+1}{n}K\rho^{1/n},
\qquad
\frac{c_s^2}{c_0^2}=\left(\frac\rho{\rho_0}\right)^{1/n}.
$$

The pseudo-enthalpy definition therefore integrates to

$$
dw=\left(\frac\rho{\rho_0}\right)^{1/n}\frac{d\rho}{\rho},
\qquad
w=n\left(\frac\rho{\rho_0}\right)^{1/n},
$$

where the constant makes $w=0$ at the surface. Thus

$$
\boxed{\rho=\rho_0n^{-n}w^n}.
$$

Hydrostatic balance is $c_0^2dw/dz=-\Omega^2z-d\Phi_d/dz$. Differentiate it, use the [Poisson equation](../../../../../../../poisson-equation.md), and set $\zeta=\Omega z/c_0$:

$$
\frac{d^2w}{d\zeta^2}
+\frac{4\pi G\rho_0}{\Omega^2}n^{-n}w^n=-1.
$$

Since the definitions in the question give $Q_0=\Omega^2/(\pi G\rho_0)$,

$$
\boxed{w''+\frac4{n^nQ_0}w^n=-1,
\qquad w(0)=n,quad w'(0)=0}.
$$

For $n=1$, put $\lambda=2/\sqrt{Q_0}$. The solution is

$$
w(\zeta)=\left(1+\frac{Q_0}{4}\right)\cos(\lambda\zeta)-\frac{Q_0}{4}.
$$

The surface $z=H$ is the first zero, so, using $c_0^2=2K\rho_0$,

$$
\boxed{
H=\frac{\sqrt{2K\rho_0Q_0}}{2\Omega}
\cos^{-1}\left(\frac{Q_0}{Q_0+4}\right)}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
