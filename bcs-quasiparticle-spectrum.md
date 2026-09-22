# BCS quasiparticle spectrum

↑ **Parent:** [BCS theory](bcs-theory.md)

The [BCS quasiparticle spectrum](bcs-quasiparticle-spectrum.md) is the positive excitation [energy](energy-split.md) obtained by diagonalizing the paired particle-hole block. Here the [weak coupling](weak-coupling.md) shell model has $\Delta\ll\Omega_D$: the minimum lies inside the pairing shell, and states outside it cost more. To derive it for a uniform isotropic real $\Delta>0$, measure the normal-state [energy](energy-split.md) from the [chemical potential](chemical-potential-split.md), $\xi_k=\epsilon_k-\mu$, and use the same sign convention as the [BCS coherence factors](bcs-coherence-factors.md):

$$
\mathcal H_k=\begin{pmatrix}\xi_k&-\Delta\\-\Delta&-\xi_k\end{pmatrix},\qquad
\det(\mathcal H_k-\varepsilon I)=\varepsilon^2-\xi_k^2-\Delta^2=0.
$$

Its [eigenvalues](eigenvalue.md) are $\varepsilon_\pm=\pm E_k$, where $E_k=\sqrt{\xi_k^2+\Delta^2}$. The positive $E_k$ is the cost of creating a [quasiparticle](quasiparticle.md) above the [BCS ground state](bcs-ground-state.md). The lower branch $-E_k$ is its particle-hole partner in this doubled matrix description, not an excitation that lowers the [ground state](ground-state.md) [energy](energy-split.md) without bound.

The location and value of the minimum follow directly:

$$
\frac{dE}{d\xi}=\frac{\xi}{\sqrt{\xi^2+\Delta^2}},\qquad
\frac{d^2E}{d\xi^2}=\frac{\Delta^2}{(\xi^2+\Delta^2)^{3/2}}>0.
$$

The unique minimum as a function of $\xi$ is $E(0)=\Delta$, at the normal-state [Fermi surface](fermi-surface.md). On an isotropic three-dimensional [Fermi surface](fermi-surface.md) it occurs for every direction of $k$, rather than at a unique point of [momentum](momentum-split.md) space. Near that minimum,

$$
E(\xi)=\Delta+\frac{\xi^2}{2\Delta}+O(\xi^4/\Delta^3).
$$

Farther away, $E(\xi)\simeq|\xi|$ when $\Delta\ll|\xi|\ll\Omega_D$. For the illustrative $\lambda=0.25$ example, a state at $\xi=\Delta$ costs $\sqrt2\Delta\simeq1.03644\ \mathrm{meV}$ rather than the minimum $0.732871\ \mathrm{meV}$.

<a id="image-opposite-momentum-cooper-pairing-opens-a-quasiparticle-gap"></a>
![](bcs-pairing-shell-and-quasiparticle-spectrum.png)

**[Figure 2](#image-opposite-momentum-cooper-pairing-opens-a-quasiparticle-gap). Opposite-momentum Cooper pairing opens a quasiparticle gap**. Original schematic section through a spherical [Fermi surface](fermi-surface.md), alongside the local isotropic [BCS quasiparticle spectrum](bcs-quasiparticle-spectrum.md). The shell thickness is exaggerated and its geometry is schematic. Both members of a shown [Cooper pair](cooper-pair.md) have nonzero opposite [momenta](momentum-split.md). The spectrum uses $x=\xi/\Delta$ only within the pairing shell; the lower branch is the redundant particle-hole partner, while positive excitations cost at least $\Delta$.

**Table of contents**

- [BCS quasiparticle](bcs-quasiparticle.md)
- [BCS electronic density of states](bcs-electronic-density-of-states.md)
- [Superconducting energy gap](superconducting-energy-gap.md)

## ↑ Ancestors (6)

1. [BCS theory](bcs-theory.md)
2. [Fermi liquid](fermi-liquid-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [BCS coherence factors](bcs-coherence-factors.md)
- [BCS quasiparticle spectrum](bcs-quasiparticle-spectrum.md)
- [Solution](past-exam-of-the-advanced-quantum-condensed-matter-physics-course-of-the-university-of-cambridge/2015/paper-1/2/c/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2017/1/a/solution.md)
- [Superconducting energy gap](superconducting-energy-gap.md)
