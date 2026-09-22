<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

**Axis theorems.** The [parallel axis theorem](../../../parallel-axis-theorem.md) states

$$
I_O=I_G+md^2,
$$

where $I_G$ is the [moment of inertia](../../../moment-of-inertia.md) about an axis through the [centre of mass](../../../center-of-mass.md), $I_O$ is about a parallel axis, $m$ is the body's total [mass](../../../mass.md), and $d$ is the perpendicular separation of the axes. Expanding $\int[(x-d)^2+y^2]dm$ proves the result because $\int x\,dm=0$ at the [centre of mass](../../../center-of-mass.md). The [perpendicular axis theorem](../../../perpendicular-axis-theorem.md) applies to a [planar lamina](../../../planar-lamina.md) in the $xy$ plane:

$$
I_z=I_x+I_y.
$$

All three axes meet at the same point, $x,y$ lie in the lamina and $z$ is normal to it; the identity follows from $x^2+y^2$ being the squared distance to the $z$ axis. It is not a theorem for an arbitrary three-dimensional body.

**Cylinder integrals.** Put the cylinder's midpoint at $z=0$ and its symmetry axis along $z$. Its uniform [mass density](../../../density.md) is $\rho=m/(\pi r^2l)$. The [transverse moment of inertia of a uniform solid cylinder](../../../transverse-moment-of-inertia-of-a-uniform-solid-cylinder.md) about the $x$ axis is

$$
I_{\perp,G}=\rho\int_{-l/2}^{l/2}dz\int_0^r s\,ds\int_0^{2\pi}d\varphi\,(z^2+s^2\sin^2\varphi)
=\frac{ml^2}{12}+\frac{mr^2}{4}.
$$

Equivalently each thin circular slice has diametral [moment of inertia](../../../moment-of-inertia.md) $r^2dm/4$, by the [perpendicular axis theorem](../../../perpendicular-axis-theorem.md) and symmetry, and shifting it by $z$ adds $z^2dm$. The [parallel axis theorem](../../../parallel-axis-theorem.md) then gives the transverse end-axis [moment of inertia](../../../moment-of-inertia.md):

$$
\boxed{I_{\perp,G}=\frac{m}{12}(l^2+3r^2),\qquad
I_{\perp,\rm end}=\frac{m}{12}(4l^2+3r^2).}
$$

The axial [moment of inertia of a uniform solid cylinder](../../../moment-of-inertia-of-a-uniform-solid-cylinder.md) is $I_\parallel=mr^2/2$. Equating it to $I_{\perp,G}$ gives

$$
\boxed{l^2=3r^2,\qquad l=\sqrt3\,r.}
$$

Here the source's principal axis means the cylinder's symmetry axis; its transverse centre axes are also [principal axes](../../../principal-axis.md). This equality describes a short cylinder rather than the thin-rod limit.

**Hammer dynamics and forces.** Treat the compact head as a [point mass](../../../point-mass.md) and neglect its intrinsic [moment of inertia](../../../moment-of-inertia.md). Let $\theta$ be the displacement from downward vertical, and let $\mathbf e_r$ point along the rod from pivot to head, with $\mathbf e_\theta$ in the direction of increasing $\theta$. Define

$$
m_T=M+m,\qquad A=Ml+\frac{ml}{2},\qquad d=\frac{A}{m_T},\qquad
I=Ml^2+m\left(\frac{l^2}{3}+\frac{r^2}{4}\right).
$$

The two external weights $Mg$ and $mg$ act at distances $l$ and $l/2$ from the pivot. The frictionless pivot supplies a reaction $\mathbf R$ but no [torque](../../../torque.md) about its axis. The total restoring [torque](../../../torque.md) and [rotational equation of motion](../../../rotational-equation-of-motion.md) are

$$
\tau=-gA\sin\theta,
\qquad \boxed{I\ddot\theta+gA\sin\theta=0.}
$$

For completeness, [Newton's second law](../../../newton-s-second-law.md) for the [centre of mass](../../../center-of-mass.md) gives both components of the pivot [force](../../../force-split.md):

$$
\boxed{R_r=-m_Td\dot\theta^2-m_Tg\cos\theta,\qquad
R_\theta=m_Td\ddot\theta+m_Tg\sin\theta.}
$$

The negative radial component points towards the pivot. These follow from the [centre of mass](../../../center-of-mass.md) [acceleration](../../../acceleration.md) $-d\dot\theta^2\mathbf e_r+d\ddot\theta\mathbf e_\theta$ and the total weight $m_Tg(\cos\theta\mathbf e_r-\sin\theta\mathbf e_\theta)$. They specify the external [forces](../../../force-split.md) even when the [oscillation](../../../oscillation.md) is not small.

With the [small-angle approximation](../../../small-angle-approximation.md), $\sin\theta\simeq\theta$, this is [simple harmonic motion](../../../simple-harmonic-motion.md). The [physical pendulum](../../../physical-pendulum.md) has small-amplitude [oscillation period](../../../period-of-an-oscillation.md)

$$
\boxed{T_0=2\pi\sqrt{\frac{I}{gA}}
=2\pi\sqrt{\frac{Ml^2+m(l^2/3+r^2/4)}{gl(M+m/2)}}.}
$$

For release from a finite amplitude $0<\theta_0<\pi$, [conservation of mechanical energy](../../../conservation-of-mechanical-energy.md) instead gives $\tfrac12I\dot\theta^2=gA(\cos\theta-\cos\theta_0)$. Integrating a quarter-cycle gives the exact [oscillation period](../../../period-of-an-oscillation.md)

$$
T(\theta_0)=4\sqrt{\frac{I}{gA}}K\!\left(\sin\frac{\theta_0}{2}\right),
\qquad K(k)=\int_0^{\pi/2}\frac{d\psi}{\sqrt{1-k^2\sin^2\psi}},
$$

where $K$ is the complete [elliptic integral of the first kind](../../../elliptic-integral-of-the-first-kind.md); $K(0)=\pi/2$ recovers $T_0$.

For $m=M/10$ and $r=l/20$, compare with the [simple pendulum](../../../simple-pendulum-split.md) value $T_s=2\pi\sqrt{l/g}$:

$$
\boxed{\frac{T_0}{T_s}
=\sqrt{\frac{1+\frac1{10}(\frac13+\frac1{1600})}{1+\frac1{20}}}
=\sqrt{\frac{49603}{50400}}\simeq0.992062.}
$$

For small [oscillations](../../../oscillation.md), the hammer's [oscillation period](../../../period-of-an-oscillation.md) is about $0.794\%$ shorter. The extra rod weight adds restoring [torque](../../../torque.md) proportionately faster than it adds pivot [moment of inertia](../../../moment-of-inertia.md).

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2021 resit](../../2021-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
