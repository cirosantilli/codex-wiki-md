# On-axis magnetic field of a circular current loop

↑ **Parent:** [Biot-Savart law](biot-savart-law.md)

A circular loop of radius $R$ carrying [electric current](electric-current.md) $I$ has, on its axis,

$$
B(z)=\frac{\mu_0IR^2}{2(R^2+z^2)^{3/2}}\,\hat z,
$$

where the sign of $\hat z$ is fixed by the [right-hand rule](right-hand-rule.md). At its centre, $B(0)=\mu_0I/(2R)$.

Put the loop in the $xy$ plane, centered at the origin, with positive [electric current](electric-current.md) counterclockwise when viewed from $+z$. The [right-hand rule](right-hand-rule.md) then gives the central [magnetic field](magnetic-field-split.md) along $+z$. Parameterize source positions by the [angle](angle.md) $\phi$ and observe at $(0,0,z)$:

$$
\mathbf r'=(R\cos\phi,R\sin\phi,0),\qquad
d\boldsymbol\ell'=R(-\sin\phi,\cos\phi,0)\,d\phi,
\qquad \mathbf R=(-R\cos\phi,-R\sin\phi,z).
$$

Here $R$ without bold type is the loop [radius](radius.md), whereas $\mathbf R$ is the source-to-observer displacement. Their [cross product](cross-product.md) is

$$
d\boldsymbol\ell'\times\mathbf R
=(Rz\cos\phi,Rz\sin\phi,R^2)\,d\phi.
$$

The denominator $|\mathbf R|^3=(R^2+z^2)^{3/2}$ is constant around the loop. The [integrals](integral-split.md) of [sine](sine.md) and [cosine](cosine.md) over a full turn vanish, while the axial contribution adds to $2\pi R^2$. Substitution into the [Biot-Savart law](biot-savart-law.md) proves the on-axis formula. [Symmetry](symmetry-physics.md) cancels transverse components; it does not cancel the axial components.

For an original one-turn example in the same vacuum approximation, choose $R=0.04\,\mathrm m$ and $I=2\,\mathrm A$. With $\mu_0\approx4\pi\times10^{-7}\,\mathrm{T\,m/A}$,

$$
B(0)=10\pi\,\mu\mathrm T\approx31.42\,\mu\mathrm T,\qquad
\frac{B(z)}{B(0)}=\left(1+\frac{z^2}{R^2}\right)^{-3/2}.
$$

At $z=0.03\,\mathrm m$, the source-to-observer distance is $0.05\,\mathrm m$, so $B(z)/B(0)=64/125=0.512$ and $B(z)\approx16.08\,\mu\mathrm T$. At $z=-0.03\,\mathrm m$, the [magnetic field](magnetic-field-split.md) has the same magnitude and still points along $+z$. The point has crossed the loop plane, but the loop's [electric current](electric-current.md) has not reversed. Reversing the [electric current](electric-current.md) reverses the [magnetic field](magnetic-field-split.md) on both sides.

<a id="image-circular-loop-magnetic-field-axial-reinforcement-and-equal-direction-on-both-sides"></a>
![](biot-savart-loop-axis-profile.png)

**[Figure 19](#image-circular-loop-magnetic-field-axial-reinforcement-and-equal-direction-on-both-sides). Circular-loop magnetic field: axial reinforcement and equal direction on both sides**. Original [electric current](electric-current.md) loop schematic and normalized on-axis calculation. The left view looks from $+z$, with counterclockwise [electric current](electric-current.md) and a central field directed toward the viewer. In the right panel, the arrows along the axis point toward $+z$ even for $z<0$; the calculated points at $z/R=\pm0.75$ have normalized field $0.512$. No experimental data are plotted.

For $|z|\ll R$, a [Taylor expansion](taylor-expansion.md) gives $B(z)/B(0)=1-3z^2/(2R^2)+O(z^4/R^4)$: the center is a smooth maximum, with zero first [derivative](derivative.md). For $|z|\gg R$,

$$
\mathbf B(z)\sim\frac{\mu_0IR^2}{2|z|^3}\widehat{\mathbf z}
=\frac{\mu_0m}{2\pi|z|^3}\widehat{\mathbf z},\qquad
m=I\pi R^2.
$$

This is the axial [magnetic dipole field](magnetic-dipole-field.md) of [magnetic dipole moment](magnetic-dipole-moment.md) $\mathbf m=I\pi R^2\widehat{\mathbf z}$.[II.14–5, equations (14.33)–(14.36): current times loop area and magnetic dipole field](the-feynman-lectures-on-physics-volume-ii-by-richard-feynman-and-others.md) A compact closed loop has an inverse-cube axial far field, in contrast to the inverse-distance field of the infinite straight wire. The [SI](international-system-of-units.md) units of the exact loop formula are $\mu_0IR^2/(R^2+z^2)^{3/2}\sim\mu_0I/\text{length}$, hence [tesla](tesla-unit.md).

For $N$ coincident turns carrying the same [electric current](electric-current.md), the [superposition principle](superposition-principle.md) multiplies the ideal result by $N$. A real coil has radial width and axial [length](length.md): if those are not negligible, integrate or sum over its individual turns. This is why a single measured coil diameter and a turn count may not determine the full spatial [magnetic field](magnetic-field-split.md) precisely. A collection of loops becomes a [solenoid](solenoid.md); integrating their axial contributions gives the [on-axis magnetic field of a finite solenoid](on-axis-magnetic-field-of-a-finite-solenoid.md).

## ↑ Ancestors (5)

1. [Biot-Savart law](biot-savart-law.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Biot-Savart law](biot-savart-law.md)
- [Current-loop torque experiment](current-loop-torque-experiment.md)
- [Far-field approximation for a current loop](far-field-approximation-for-a-current-loop.md)
- [Force between distant coaxial current loops](force-between-distant-coaxial-current-loops.md)
- [Helmholtz coil](helmholtz-coil.md)
- [On-axis magnetic field of a finite solenoid](on-axis-magnetic-field-of-a-finite-solenoid.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/15d/c/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-1/section-b/b8/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-1/section-b/b8/solution.md)
- [Uniformly magnetized cylinder](uniformly-magnetized-cylinder.md)
