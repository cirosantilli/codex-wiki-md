# Lattice constant from two indexed reflections

↑ **Parent:** [X-ray crystallographic structure inference](x-ray-crystallographic-structure-inference.md)

Choose an original simulated model: a [primitive cubic lattice](primitive-cubic-lattice.md) with one identical point scatterer per [primitive unit cell](primitive-unit-cell.md), edge $a=0.400\,\mathrm{nm}$, and incident [X-ray](x-ray.md) [wavelength](wavelength.md) $\lambda=0.200\,\mathrm{nm}$. These are stipulated lengths, not measurements of [sodium chloride](sodium-chloride.md). Suppose orientation information has already assigned the two observed reflections the [Miller indices](miller-index.md) $(100)$ and $(110)$. The detector deflection is $2\theta$, where $\theta$ is the [Bragg angle](bragg-angle.md).

Use the existing [interplanar spacing](interplanar-spacing.md) formula and [Bragg's law](bragg-s-law.md), with higher [diffraction orders](diffraction-order.md) absorbed into the reflection indices:

$$
N=h^2+k^2+l^2,\qquad d_{hkl}=\frac{a}{\sqrt N},\qquad
\sin^2\theta_{hkl}=\frac{\lambda^2}{4a^2}N,\qquad
a=\frac{\lambda\sqrt N}{2\sin\theta_{hkl}}.
$$

The simulated $(100)$ reflection has $\sin\theta=1/4$, hence $2\theta=28.9550^\circ$. The $(110)$ reflection has $\sin\theta=\sqrt2/4$, hence $2\theta=41.4096^\circ$. Their squared [sines](sine.md) are $0.0625$ and $0.125$, in ratio $1:2$. Substituting the unrounded angles independently gives

$$
a_{100}=\frac{0.200}{2(1/4)}=0.400\,\mathrm{nm},\qquad
a_{110}=\frac{0.200\sqrt2}{2(\sqrt2/4)}=0.400\,\mathrm{nm}.
$$

Agreement tests a proposed indexing and scale together; disagreement would prompt checks of the indexing, [wavelength](wavelength.md), angular zero, or the assumed [unit cell](unit-cell.md) geometry.

<a id="image-x-ray-two-peak-lattice-inference"></a>
![](x-ray-two-peak-lattice-inference.png)

**[Figure 2](#image-x-ray-two-peak-lattice-inference). Two indexed reflections recover the same cubic repeat length**. Original simulation with $a=0.400\,\mathrm{nm}$ and $\lambda=0.200\,\mathrm{nm}$. Left: selected $(100)$ and $(110)$ positions on a detector-deflection axis; equal stick heights are only markers. Right: their squared [sines](sine.md) lie on the line of slope $\lambda^2/(4a^2)=1/16$. These are selected reflections, not a complete scan, a powder trace, or measured [sodium chloride](sodium-chloride.md) data.

Two peak positions alone do not establish the indexing. Assigning the same two angles to $(110)$ and $(200)$ would give $N=2,4$ and $a=0.400\sqrt2\simeq0.565685\,\mathrm{nm}$ instead. More reflections, orientation information and [systematic absences](systematic-absence.md) help discriminate such assignments. An unobserved reflection can be inaccessible, weak or extinguished by the [atomic basis](atomic-basis-of-a-crystal.md); absence is not automatically evidence for a larger [interplanar spacing](interplanar-spacing.md).

Absolute scale also requires [measurement calibration](measurement-calibration.md) of the [wavelength](wavelength.md). To first order, [differentiation](differentiation.md) of the inferred length gives

$$
\frac{\delta a}{a}=\frac{\delta\lambda}{\lambda}-\cot\theta\,\delta\theta,
$$

with angular changes in [radians](radian.md). A stipulated detector-zero error $\delta(2\theta)=+0.100^\circ$, with correct [wavelength](wavelength.md), biases the first inferred edge downward by approximately $0.338\%$ and the second by $0.231\%$. A common angular offset therefore need not cancel when two inferred lengths are compared. These are model sensitivity estimates, not historical instrument uncertainties.

## ↑ Ancestors (6)

1. [X-ray crystallographic structure inference](x-ray-crystallographic-structure-inference.md)
2. [Crystallography](crystallography.md)
3. [Crystal structure](crystal-structure.md)
4. [Physical chemistry](physical-chemistry-split.md)
5. [Chemistry](chemistry-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [X-ray crystallographic structure inference](x-ray-crystallographic-structure-inference.md)
