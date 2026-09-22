# Uniformly magnetized cylinder

↑ **Parent:** [Magnetization](magnetization.md)

Prescribe constant [magnetization](magnetization.md) $\mathbf M=M\widehat{\mathbf z}$, with $M>0$, inside a [circular cylinder](circular-cylinder.md) of [radius](radius.md) $R$ and [length](length.md) $L$, surrounded by zero [magnetization](magnetization.md). In [cylindrical coordinates](cylindrical-coordinate-system.md), the outward [unit normal](unit-normal.md) on the curved [surface](topological-surface-split.md) is $\widehat{\mathbf r}$, so

$$
\mathbf J_{\rm b}=\mathbf0\quad\text{in the interior},\qquad
\mathbf K_{\rm b}=M\widehat{\mathbf z}\times\widehat{\mathbf r}
=M\widehat{\boldsymbol\phi}\quad\text{on the side}.
$$

The endcaps have outward [unit normals](unit-normal.md) $+\widehat{\mathbf z}$ and $-\widehat{\mathbf z}$. Their [cross products](cross-product.md) with [magnetization](magnetization.md) vanish, so $\mathbf K_{\rm b}=0$ on each endcap. The side [bound current](bound-current.md) circulates counterclockwise when viewed from $+z$, by the [right-hand rule](right-hand-rule.md). Zero endcap [surface current density](surface-current-density.md) does not imply zero endcap [magnetic field](magnetic-field-split.md).

<a id="image-a-uniformly-magnetized-circular-cylinder-is-equivalent-to-a-circumferential-bound-current-sheet"></a>
![](magnetized-cylinder-bound-current-geometry.png)

**[Figure 7](#image-a-uniformly-magnetized-circular-cylinder-is-equivalent-to-a-circumferential-bound-current-sheet). A uniformly magnetized circular cylinder is equivalent to a circumferential bound current sheet**. Original prescribed-[magnetization](magnetization.md) geometry. Blue arrows represent $\mathbf M$; orange arrows represent side [surface current density](surface-current-density.md), not independent wires. The end view looks from $+z$. The endcap [unit normals](unit-normal.md) are parallel or antiparallel to $\mathbf M$, so neither endcap carries [bound current](bound-current.md). The drawing specifies source geometry, not a uniform finite-cylinder [magnetic field](magnetic-field-split.md).

For an original example, let $M=800\,\mathrm{A/m}$, $R=0.020\,\mathrm m$, and $L=0.10\,\mathrm m$. The [volume](volume.md) and total [magnetic dipole moment](magnetic-dipole-moment.md) are

$$
V=\pi R^2L=4\pi\times10^{-5}\,\mathrm{m^3},\qquad
\mathbf m=MV\widehat{\mathbf z}
=0.032\pi\,\mathrm{A\,m^2}\widehat{\mathbf z}
\approx0.100531\,\mathrm{A\,m^2}\widehat{\mathbf z}.
$$

Check the result independently using the equivalent [bound current](bound-current.md): a side strip of axial [length](length.md) $dz$ forms a [current loop](current-loop.md) with $dI=M\,dz$ and [magnetic dipole moment](magnetic-dipole-moment.md) $d\mathbf m=\pi R^2M\,dz\,\widehat{\mathbf z}$. Its [integral](integral-split.md) over $L$ gives the same $M\pi R^2L\widehat{\mathbf z}$. In particular, $ML=80\,\mathrm A$ is the sum of the equivalent loop [electric currents](electric-current.md) across a full axial cut; it is not a [surface current density](surface-current-density.md).

The side [surface current density](surface-current-density.md) has exactly the geometry of a continuum [solenoid](solenoid.md) with $nI=M$, where $n$ is [solenoid turn density](solenoid-turn-density.md). In the infinite-cylinder idealization with no applied [magnetic field](magnetic-field-split.md), the [long-solenoid approximation](long-solenoid-approximation.md) therefore becomes

$$
\mathbf B_{\rm in}=\mu_0M\widehat{\mathbf z},\qquad
\mathbf B_{\rm out}=\mathbf0,\qquad\mathbf H=\mathbf0.
$$

The [limit](limit-of-a-function.md) is useful well away from the ends of a sufficiently long [circular cylinder](circular-cylinder.md). A finite [circular cylinder](circular-cylinder.md) instead has fringing [magnetic field](magnetic-field-split.md) and a [demagnetizing field](demagnetizing-field.md). For this prescribed uniform [magnetization](magnetization.md), integrate the [on-axis magnetic field of a circular current loop](on-axis-magnetic-field-of-a-circular-current-loop.md), or substitute $nI=M$ in the [on-axis magnetic field of a finite solenoid](on-axis-magnetic-field-of-a-finite-solenoid.md), to obtain the central [magnetic field](magnetic-field-split.md):

$$
B_z(0)=\mu_0M\frac{L}{\sqrt{L^2+4R^2}}.
$$

Our example has $L/(2R)=2.5$ and $B_z(0)/(\mu_0M)=5/\sqrt{29}\approx0.92848$, rather than unity. With the rounded [vacuum permeability](vacuum-permeability.md) $\mu_0\approx4\pi\times10^{-7}\,\mathrm{T\,m/A}$, this is approximately $0.9334\,\mathrm{mT}$, compared with the infinite-cylinder value $1.0053\,\mathrm{mT}$. These are model calculations for a prescribed [magnetization](magnetization.md), not measured values or a solution for the self-consistent [magnetization](magnetization.md) of an arbitrary material.

## ↑ Ancestors (6)

1. [Magnetization](magnetization.md)
2. [Bound charge and bound current](bound-charge-and-bound-current.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
