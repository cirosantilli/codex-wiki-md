<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\mathbf u=u(y,t)\mathbf e_x$, [incompressibility](../../../../../incompressible-flow.md) is automatic and the nonlinear advection term is zero. With no [pressure](../../../../../pressure-split.md) gradient the streamwise momentum equation is $\boxed{\rho u_t=\mu u_{yy}}$. Seek its periodic response as $u=\operatorname{Re}[Uf(y)e^{i\Omega t}]$. The amplitude satisfies $f''=i\rho\Omega f/\mu$ with $f(\pm d)=1$. Since $[k(1+i)]^2=i\rho\Omega/\mu$ for $k=\sqrt{\rho\Omega/(2\mu)}$, even symmetry gives

$$
\boxed{f(y)=\frac{\cosh[k(1+i)y]}{\cosh[k(1+i)d]}.}
$$

Odd components vanish because the two boundary amplitudes are equal. This is the unique periodic solution. Without a specified initial profile, decaying zero-wall diffusion transients may be added, so the formula should not be read as a claim that every transient is absent.

As $kd\to\infty$, the wall motions penetrate only a distance $k^{-1}=\sqrt{2\mu/(\rho\Omega)}$. Near either wall, with inward distance $s=d-|y|$, the leading [velocity](../../../../../velocity.md) is

$$
\boxed{u\sim Ue^{-ks}\cos(\Omega t-ks).}
$$

The two oscillatory viscous layers are separated by an almost motionless core; the phase lag increases inward. This is [in-phase oscillating parallel-plate flow](../../../../../in-phase-oscillating-parallel-plate-flow.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
