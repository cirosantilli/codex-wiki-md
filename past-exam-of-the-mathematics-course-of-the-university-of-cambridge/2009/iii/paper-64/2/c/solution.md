<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Matter corotating with the footpoint has fixed [angular velocity](../../../../../../angular-velocity.md) $\Omega_0=(GM/R_0^3)^{1/2}$. Its [effective potential](../../../../../../effective-potential.md) in that rotating frame is the sum of [Newtonian gravitational potential](../../../../../../newtonian-gravitational-potential.md) and centrifugal potential,

$$
\Phi_{\rm eff}(R,z)=-\frac{GM}{\sqrt{R^2+z^2}}-\frac12\Omega_0^2R^2.
$$

Along an outward-inclined straight [magnetic field line](../../../../../../magnetic-field-line.md), write $R=R_0+s\sin i$ and $z=s\cos i$, where $s$ is distance from the footpoint. The exact potential along it is

$$
\Phi_{\rm eff}(s)=-\frac{GM}{\sqrt{R_0^2+2R_0s\sin i+s^2}}-\frac{GM}{2R_0^3}(R_0+s\sin i)^2.
$$

Its first [derivative](../../../../../../derivative.md) at $s=0$ is zero by the [Keplerian rotation](../../../../../../keplerian-disk.md) balance. At the footpoint the meridional [Hessian](../../../../../../hessian-matrix.md) is $\operatorname{diag}(-3\Omega_0^2,\Omega_0^2)$ with zero mixed derivative. Hence

$$
\boxed{\Phi_{\rm eff}(s)=-\frac{3GM}{2R_0}+\frac12\Omega_0^2(1-4\sin^2i)s^2+O(\Omega_0^2s^3/R_0).}
$$

When $0\leq i<30^\circ$, the potential initially rises and a cold parcel must overcome a barrier. When $i>30^\circ$, its quadratic curvature is negative, so the footpoint is a local maximum along the field and a small outward [displacement](../../../../../../displacement.md) is accelerated further outward:

$$
\boxed{-\frac{d\Phi_{\rm eff}}{ds}=\Omega_0^2(4\sin^2i-1)s+O(\Omega_0^2s^2/R_0)>0\quad(s>0\text{ small},\ i>30^\circ).}
$$

This is the [thirty-degree magnetocentrifugal launching criterion](../../../../../../thirty-degree-magnetocentrifugal-launching-criterion.md). It describes the lack of a local cold-launch barrier, not a nonzero force on a parcel exactly at rest at $s=0$. At exactly $30^\circ$ the quadratic term vanishes; for the specified straight line the next term is $-7\Omega_0^2s^3/(16R_0)$, as in [marginal straight-line launch at thirty degrees](../../../../../../marginal-straight-line-launch-at-thirty-degrees.md). Global wind escape additionally depends on conditions farther along the line.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
