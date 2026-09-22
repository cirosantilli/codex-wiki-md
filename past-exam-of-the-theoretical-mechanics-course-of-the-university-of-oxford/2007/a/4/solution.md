<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Two-dimensional [incompressibility](../../../../incompressible-flow.md) permits $u=\psi_y$, $v=-\psi_x$. Taking the [curl](../../../../curl.md) of the Stokes momentum equation eliminates [pressure](../../../../pressure-split.md) and gives $\nabla^2(v_x-u_y)=0$. Since $v_x-u_y=-\nabla^2\psi$, the [stream function](../../../../stream-function.md) obeys $\boxed{\nabla^4\psi=0}$.

Scale radius by $a$, [velocity](../../../../velocity.md) by $U$ and [stream function](../../../../stream-function.md) by $Ua$. In [polar coordinates](../../../../polar-coordinates.md) $u_r=r^{-1}\psi_\theta$, $u_\theta=-\psi_r$. No penetration makes $\psi$ constant on the cylinder; choose that constant zero. No slip also requires $\psi_r=0$ at $r=1$. The uniform stream has $\psi=r\sin\theta$, specifying the far-field condition.

The boundary forcing has angular mode $\sin\theta$, so its corresponding mode must have $\psi=f(r)\sin\theta$. Define $L_1=d^2/dr^2+r^{-1}d/dr-r^{-2}$. Then $\nabla^4\psi=(L_1^2f)\sin\theta$, while $L_1r^s=(s^2-1)r^{s-2}$. Thus the [indicial equation](../../../../indicial-equation.md) of $L_1^2$ is $(s^2-1)[(s-2)^2-1]=(s-3)(s-1)^2(s+1)=0$, giving

$$
\boxed{f=Ar^3+Br\log r+Cr+Dr^{-1}.}
$$

The repeated exponent one supplies the logarithmic term. The condition $f'\to1$ first forces $A=B=0$ and $C=1$. Then $f(1)=0$ forces $D=-1$, but $f'(1)=C-D=2\ne0$. No additional [Fourier mode](../../../../fourier-mode.md) can repair the missing [boundary condition](../../../../boundary-condition.md) in this angular mode. Therefore the unbounded-domain Stokes problem has no solution with both no slip and a nonzero uniform far stream.

This is [Stokes' paradox](../../../../stokes-paradox.md). It identifies a nonuniform approximation, rather than the absence of physical flow. For any small but nonzero [Reynolds number](../../../../reynolds-number.md), convective inertia becomes important sufficiently far away. An inner Stokes region must be matched to an outer Oseen or Navier-Stokes region that retains that inertia. Alternatively, finite external boundaries introduce a different well-posed physical problem; they cannot be sent to infinity while keeping the naive Stokes solution unchanged.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
