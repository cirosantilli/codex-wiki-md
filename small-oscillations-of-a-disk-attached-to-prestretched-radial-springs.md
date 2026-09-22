# Small oscillations of a disk attached to prestretched radial springs

↑ **Parent:** [Small oscillation](small-oscillation.md)

A uniform [rigid body](rigid-body-dynamics-split.md) disk of [mass](mass.md) $m$ and radius $a$ moves in a frictionless plane. Let $N\ge3$ identical [springs](spring.md) attach equally spaced rim points to fixed anchors in their radial directions. The equilibrium spring length is $l$, natural length $l_0<l$, and [spring constant](spring-constant.md) $k$. Write the small centre [displacement](displacement.md) as $\mathbf q$ and the rotation as $\theta$. For a spring with radial and tangential unit [vectors](vector.md) $\mathbf n,\mathbf t$, its length is

$$
s=l-\mathbf n\cdot\mathbf q+\frac a2\theta^2+
\frac{(\mathbf t\cdot\mathbf q+a\theta)^2}{2l}+O((|\mathbf q|+|\theta|)^3).
$$

This follows by a second-order [Taylor series](taylor-series.md) for the distance between $\mathbf q+aR(\theta)\mathbf n$ and $(a+l)\mathbf n$. In the [elastic potential energy](elastic-energy.md) $k(s-l_0)^2/2$, the equilibrium tension $k\tau$ multiplies the second-order change of length. Thus it contributes to the linearized stiffness even though the displacement is small.

The equally spaced directions satisfy $\sum\mathbf n=\sum\mathbf t=0$ and $\sum\mathbf n\mathbf n^T=\sum\mathbf t\mathbf t^T=(N/2)I$. Summing the spring energies gives

$$
V_2=\frac{Nk}{4}(1+\tau/l)|\mathbf q|^2+\frac{Nk\tau a(a+l)}{2l}\theta^2.
$$

The [kinetic energy](kinetic-energy.md) is $m|\dot{\mathbf q}|^2/2+ma^2\dot\theta^2/4$, using the [moment of inertia of a uniform disc](moment-of-inertia-of-a-uniform-disc.md). The [Euler-Lagrange equations](euler-lagrange-equation.md) give the displayed squared [angular frequencies](angular-frequency.md). The translational [normal modes](normal-mode.md) are degenerate; rotation is independent. At zero prestretch the rotational frequency vanishes at quadratic order, and finite-angle spring stretching first contributes at higher order.

<a id="image-translations-and-rotation-of-a-disk-attached-to-symmetric-prestretched-radial-springs"></a>
![](radially-sprung-disk-normal-modes.png)

**[Figure 2](#image-translations-and-rotation-of-a-disk-attached-to-symmetric-prestretched-radial-springs). Translations and rotation of a disk attached to symmetric prestretched radial springs**.

## ↑ Ancestors (6)

1. [Small oscillation](small-oscillation.md)
2. [Lagrangian mechanics](lagrangian-mechanics-split.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-2/7/c/solution.md)
