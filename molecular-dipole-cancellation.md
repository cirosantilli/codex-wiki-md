# Molecular dipole cancellation

↑ **Parent:** [Bond dipole](bond-dipole.md)

[Molecular dipole cancellation](molecular-dipole-cancellation.md) occurs when nonzero contributions to a [molecule](molecule-split.md)'s [electric dipole moment](electric-dipole-moment.md) cancel under [vector addition](vector-addition.md). In a [bond dipole](bond-dipole.md) model, use $\mathbf p_{\rm mol}=\sum_b\mathbf p_b$; adding magnitudes instead discards the [molecular geometry](molecular-geometry.md). A symmetric [linear molecule](linear-molecule.md) with two equivalent opposed [bond dipoles](bond-dipole.md) has $\mathbf p_1=p_0\widehat{\mathbf x}$ and $\mathbf p_2=-p_0\widehat{\mathbf x}$, hence zero total [electric dipole moment](electric-dipole-moment.md) even though each [chemical bond](chemical-bond-split.md) is polarized. [Carbon dioxide](carbon-dioxide.md) provides the familiar molecular example; [water](water.md)'s [bent molecular geometry](bent-molecular-geometry.md) permits a nonzero total.[§7.6, Figure 7.27 and accompanying paragraphs: cancellation in carbon dioxide, noncancellation in water](chemistry-2e-by-paul-flowers-and-others.md)

For an original geometry calculation, give a fictitious three-site model $AB_2$ a central effective [electric charge](electric-charge-split.md) $+2q$ at the origin and two terminal [electric charges](electric-charge-split.md) $-q$ at

$$
\mathbf r_1=r\bigl(-\sin(\theta/2),\cos(\theta/2)\bigr),\qquad
\mathbf r_2=r\bigl(\sin(\theta/2),\cos(\theta/2)\bigr),\qquad 0<\theta\leq\pi.
$$

Here $r$ is the stipulated [bond length](bond-length.md), $\theta$ the [angle](angle.md) between the two connections, and $q>0$ is independent of any [electronegativity](electronegativity-split.md) scale. Equivalently, split the central $+2q$ into two colocated $+q$ contributions, one for each neutral [bond dipole](bond-dipole.md). With $p_0=qr$, the physical [electric dipole moments](electric-dipole-moment.md) point from the terminal sites towards the central site:

$$
\begin{aligned}
\mathbf p_1&=p_0\bigl(\sin(\theta/2),-\cos(\theta/2)\bigr),\\
\mathbf p_2&=p_0\bigl(-\sin(\theta/2),-\cos(\theta/2)\bigr),\\
\mathbf p_{\rm mol}&=\mathbf p_1+\mathbf p_2
=\bigl(0,-2p_0\cos(\theta/2)\bigr).
\end{aligned}
$$

The sideways components cancel; the components along the [angle bisector](angle-bisector.md) add. Thus $|\mathbf p_{\rm mol}|=2p_0\cos(\theta/2)$. At $\theta=180^\circ$ the result is zero; at the stipulated $\theta=120^\circ$ it is exactly $p_0$. This is an angle example for a model, not the measured angle or [electric dipole moment](electric-dipole-moment.md) of [water](water.md).

<a id="image-molecular-dipole-components-and-cancellation"></a>
![](molecular-dipole-components-and-cancellation.png)

**[Figure 7](#image-molecular-dipole-components-and-cancellation). Vector addition of physical bond dipoles in a stipulated neutral three-site model: cancellation at $180^\circ$, a bisector resultant at $120^\circ$**. Central effective [electric charge](electric-charge-split.md) $+2q$, terminal [electric charges](electric-charge-split.md) $-q$, and equal [bond lengths](bond-length.md) $r$. Arrows point from negative to positive [electric charge](electric-charge-split.md). The lower panels translate the [bond dipoles](bond-dipole.md) to a common origin and show their components; they are vectors, not electron trajectories or extra bonds.

Opposition alone is insufficient: a [linear molecule](linear-molecule.md) with unequal opposed [bond dipoles](bond-dipole.md) of magnitudes $p_1$ and $p_2$ retains magnitude $|p_1-p_2|$. Conversely, symmetry can enforce exact cancellation beyond a particular [bond dipole](bond-dipole.md) partition. If the complete [charge density](charge-density.md) invariant under [point reflection](point-reflection.md) about the origin satisfies $\rho(\mathbf r)=\rho(-\mathbf r)$, contributions to $\int\mathbf r\rho(\mathbf r)\,d^3r$ cancel in pairs. That [proof](mathematical-proof.md) uses the whole [electric charge](electric-charge-split.md) distribution, including [lone pairs](lone-pair.md) and [atomic nuclei](atomic-nucleus-split.md). It explains why molecular [symmetry](symmetry-physics.md) is stronger evidence for zero permanent [electric dipole moment](electric-dipole-moment.md) than a rule based only on tabulated [electronegativity](electronegativity-split.md) differences.

A permanent molecular [electric dipole moment](electric-dipole-moment.md) is specified relative to the [molecule](molecule-split.md)'s orientation. An ensemble with random orientations can have zero mean laboratory [vector](vector.md) while each [molecule](molecule-split.md) is polar. That orientational average differs from internal [molecular dipole cancellation](molecular-dipole-cancellation.md). The [Stark effect](stark-effect.md) and [molecular beam electric resonance](molecular-beam-electric-resonance.md) probe molecular [electric dipole moments](electric-dipole-moment.md) through state-dependent responses to an [electric field](electric-field-split.md).

## ↑ Ancestors (6)

1. [Bond dipole](bond-dipole.md)
2. [Bond polarization](bond-polarization.md)
3. [Electronegativity](electronegativity-split.md)
4. [Chemical bond](chemical-bond-split.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Molecular dipole cancellation](molecular-dipole-cancellation.md)
- [Polar covalent bond](polar-covalent-bond.md)
