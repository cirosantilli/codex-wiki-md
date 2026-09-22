<h1 id="9b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\theta=0$ initially and choose its positive sense to agree with the initial tangential motion. The inward radial component is $\dot r(0)=-4\cos(\pi/3)=-2$, while the tangential [speed](../../../../../../speed.md) is $4\sin(\pi/3)=2\sqrt3$. Hence

$$
\boxed{l=2\sqrt3,\quad u(0)=1,\quad u'(0)=1/\sqrt3.}
$$

Substitution in the [Binet equation](../../../../../../binet-equation.md) gives $12(u''+u)=3+9u$, or $u''+u/4=1/4$. This is an [orbit equation for combined inverse-square and inverse-cube attraction](../../../../../../orbit-equation-for-combined-inverse-square-and-inverse-cube-attraction.md). Solving the constant-coefficient equation and applying both initial conditions gives

$$
\boxed{u(\theta)=1+\frac2{\sqrt3}\sin(\theta/2).}
$$

On $0\leq\theta\leq2\pi$, the sine is nonnegative, so $r$ stays finite and positive. At $\theta=2\pi$, $u=1$, hence $r=1$ and the particle is back at its original spatial position after one revolution. But $u'(2\pi)=-1/\sqrt3$, so its radial [velocity](../../../../../../velocity.md) is now $+2$, rather than the original $-2$. **The return is not a periodic return in position and [velocity](../../../../../../velocity.md).**

After that revolution, the first zero of $u$ is at $\theta=8\pi/3$, where $\sin(\theta/2)=-\sqrt3/2$. The physical branch therefore has $r\to\infty$ as $\theta\uparrow8\pi/3$; it must not be continued into negative $u$. Since $dt/d\theta=1/(lu^2)$ and $u$ has a simple zero, reaching infinity takes infinite time. As a check, the specific [potential energy](../../../../../../potential-energy.md) is $\Phi(r)=-3/r-9/(2r^2)$ and the conserved energy per unit [mass](../../../../../../mass.md) is $4^2/2+\Phi(1)=1/2$, giving escape [speed](../../../../../../speed.md) $1$ at infinity, also obtained from $-lu'(8\pi/3)=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9B](../../9b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
