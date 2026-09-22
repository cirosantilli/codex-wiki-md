<h1 id="37e/solution">Solution</h1>

↑ **Parent:** [37E](../37e.md)

Incompressibility gives $r^{-1}(ru)_r+r^{-1}v_\phi=0$, permitting a [stream function](../../../../../stream-function.md) with $u=\psi_\phi/r$, $v=-\psi_r$. Its axial vorticity is $-\Delta\psi$. Taking the curl of the [Stokes flow](../../../../../stokes-flow-split.md) momentum equation eliminates pressure and gives $\Delta$ of that vorticity zero, hence $\Delta^2\psi=0$.

At an impermeable constant-angle plane, $v=0$ means $\psi$ is constant along that boundary. Fix that constant to zero. A rigid boundary also requires $\psi_\phi=0$. The tangential stress is $\mu(-\psi_{rr}+\psi_r/r+\psi_{\phi\phi}/r^2)$; along an impermeable boundary its first two terms vanish, so a stress-free boundary requires $\psi_{\phi\phi}=0$.

Write $\psi=(S/\mu)r^2F(\phi)$. The [biharmonic equation](../../../../../biharmonic-equation.md) becomes $F''''+4F''=0$. The [boundary conditions](../../../../../boundary-condition.md) are $F(-\alpha)=F'(-\alpha)=F(0)=0$ and $F''(0)=1$. Consequently

$$
F=\tfrac14(1-\cos2\phi)+B\phi+D\sin2\phi,
$$



$$
D=\frac{1-\cos2\alpha-2\alpha\sin2\alpha}{4(\sin2\alpha-2\alpha\cos2\alpha)},\qquad B=\tfrac12\sin2\alpha-2D\cos2\alpha.
$$

The requested $f$ is $F/\mu$. Evaluating $u(r,0)=(Sr/\mu)F'(0)$ gives

$$
\boxed{U(r)=\frac{Sr}{\mu}\frac{1-\cos2\alpha-\alpha\sin2\alpha}{\sin2\alpha-2\alpha\cos2\alpha}.}
$$

Its small-angle ratio is $\alpha/4+O(\alpha^3)$, so $U$ and $S$ have the same sign for sufficiently small positive angle. At the first nonzero critical root, $2\alpha_c\simeq4.493409$, the denominator vanishes while the numerator does not. The pure $r^2$ similarity solution is then resonant and cannot satisfy the forcing; logarithmic radial terms or additional global boundary data are needed. Just beyond this angle, and up to $\alpha<\pi$, the denominator is negative and numerator positive, so the formal surface flow reverses relative to $S$. This is not a contradiction of viscous dissipation: the wedge is radially unbounded and its radial-end energy flux has not been prescribed. A physical finite-domain flow needs those outer conditions, and the Stokes approximation also fails sufficiently far out when the velocity grows with $r$.

## ↑ Ancestors (10)

1. [37E](../37e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
