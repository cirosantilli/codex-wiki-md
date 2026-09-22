<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [two-pair component of polarization-entangled down-conversion](../../../../two-pair-component-of-polarization-entangled-down-conversion.md) to account for identical [bosons](../../../../boson.md) in the same collected modes. Write $a_H^\dagger$ for a [creation operator](../../../../creation-operator.md) in mode $a$ with [horizontal polarization](../../../../horizontal-polarization.md), and similarly for the other modes. For the plus [Bell state](../../../../bell-state-split.md), the pair-creation operator is $K^\dagger=a_H^\dagger b_V^\dagger+a_V^\dagger b_H^\dagger$. The normalized four-photon state is

$$
|\Psi_2\rangle=\frac{(K^\dagger)^2}{2\sqrt3}|0\rangle
=\frac{|2H_a,2V_b\rangle+|H_aV_a,H_bV_b\rangle+|2V_a,2H_b\rangle}{\sqrt3}.
$$

These are normalized [Fock states](../../../../fock-state.md). In particular, $(a_H^\dagger)^2|0\rangle=\sqrt2|2H_a\rangle$; omitting this factor would misnormalize the four-photon input.

The first [polarizing beam splitter](../../../../polarizing-beam-splitter.md) sends $a_H^\dagger$ to $T_H^\dagger$ and $a_V^\dagger$ to $c_V^\dagger$. Only the middle term can give exactly one trigger photon and leave another photon in $c$. In the first term both $a$ photons reach $T$ and none reaches $c$; in the last there is no trigger. Thus the relevant, still unnormalized component is

$$
\frac1{\sqrt3}T_H^\dagger c_V^\dagger b_H^\dagger b_V^\dagger|0\rangle.
$$

For the selected paths of the [half-wave plate](../../../../half-wave-plate.md) and [beam splitter](../../../../beam-splitter.md), take

$$
c_V^\dagger\longmapsto\frac{c_H^{\prime\dagger}+c_V^{\prime\dagger}}{\sqrt2},\qquad
b_\sigma^\dagger\longmapsto\frac{d_\sigma^\dagger+e_\sigma^\dagger}{\sqrt2},\quad\sigma=H,V.
$$

Here $e$ labels the output towards $D_3$. An immaterial common reflection phase has been absorbed in the mode definitions. Keeping one photon at $D_3$ leaves

$$
\frac{T_H^\dagger}{2\sqrt6}
(c_H^{\prime\dagger}+c_V^{\prime\dagger})
(d_H^\dagger e_V^\dagger+d_V^\dagger e_H^\dagger)|0\rangle.
$$

At the final [polarizing beam splitter](../../../../polarizing-beam-splitter.md), the $H_{c'}H_d$ alternative yields one $H$ at each of $D_1,D_2$, while $V_{c'}V_d$ yields one $V$ at each. The two opposite-polarization alternatives send both photons to the same detector and fail fourfold [coincidence counting](../../../../coincidence-counting.md). The accepted component is therefore

$$
\frac1{2\sqrt6}|H\rangle_T
\bigl(|HHV\rangle_{123}+|VVH\rangle_{123}\bigr).
$$

After conditioning and [normalization](../../../../normalization.md), the three detected output modes have

$$
\boxed{|\mathrm{GHZ}\rangle_{123}=\frac{|VVH\rangle+|HHV\rangle}{\sqrt2}.}
$$

The [optical mode matching](../../../../optical-mode-matching.md) must erase any timing, frequency or other record that distinguishes the two alternatives. Otherwise the same polarization populations could describe an incoherent [mixed quantum state](../../../../mixed-state.md), rather than this [quantum superposition](../../../../quantum-superposition.md). The [Bouwmeester three-photon GHZ experiment](../../../../bouwmeester-three-photon-ghz-experiment.md) uses this principle. The [photonic GHZ preparation by fourfold coincidence](../../../../photonic-ghz-preparation-by-fourfold-coincidence.md) is a measurement in the coincidence basis: detecting all four photons projects and consumes them. A click at $T$ by itself does not herald a guaranteed freely available three-photon state.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [8](../../8-split.md)
3. [2010](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
