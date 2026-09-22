<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To first order, vanishing tangential velocity on the [elastic plate](../../../../../../elastic-plate.md) is simply $u(0)=0$. In the mode from part a this gives

$$
C=-kA.
$$

Consequently

$$
u=k^2Az\,e^{kz}e^{ikx},
\qquad
w=ikA(1-kz)e^{kz}e^{ikx},
$$

so $u(0)=0$, $w(0)=ikA e^{ikx}$, and $w_z(0)=0$. The dynamic pressure at the surface is

$$
p'(0)=-2i\mu k^2A e^{ikx}
=-2\mu k\,w(0).
$$

Evaluating the hydrostatic pressure at $z=\zeta$ contributes the restoring normal stress $\rho g\zeta$. Since $\nabla^4\zeta=k^4\zeta$ for this mode, the linearized normal-stress balance is

$$
\rho g\zeta-p'(0)+2\mu w_z(0)+Bk^4\zeta=0.
$$

It follows that

$$
\boxed{u(x,0,t)=0},
$$



$$
\boxed{
w(x,0,t)
=-\frac{\rho g+Bk^4}{2\mu k}\,
\epsilon(t)e^{ikx}}.
$$

The two restoring effects are buoyancy and the plate's [bending stiffness](../../../../../../bending-stiffness.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
