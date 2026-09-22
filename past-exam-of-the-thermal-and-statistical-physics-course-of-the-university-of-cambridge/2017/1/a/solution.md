<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\xi=\epsilon-\epsilon_F$ and $\Delta=|\Delta|>0$. The [BCS quasiparticle spectrum](../../../../bcs-quasiparticle-spectrum.md) has $E=\sqrt{\xi^2+\Delta^2}$, so on either inverse branch

$$
\xi_\pm=\pm\sqrt{E^2-\Delta^2},\qquad
\left|\frac{d\xi_\pm}{dE}\right|=\frac E{\sqrt{E^2-\Delta^2}}.
$$

Conservation of states on one branch gives $D_{\rm branch}(E)dE=g(\epsilon_F)|d\xi|$. Consequently the single-branch expression requested in the source is

$$
\boxed{D_{\rm branch}(E)=\frac{g(\epsilon_F)E}{\sqrt{E^2-\Delta^2}},\qquad E>\Delta.}
$$

There are no such states for $0<E<\Delta$ in this ideal fully gapped model. Near the edge the [density of states](../../../../density-of-states.md) diverges as $(E-\Delta)^{-1/2}$, an integrable singularity; at large $E/\Delta$ it approaches its normal-state value.

**Counting qualification.** The [energy](../../../../energy-split.md) map in the source is two-to-one. If $g(\epsilon)$ literally counts all normal-state levels both above and below $\epsilon_F$, the unweighted [positive-energy quasiparticle density from a folded spectrum](../../../../positive-energy-quasiparticle-density-from-a-folded-spectrum.md) must sum both preimages, and is instead

$$
\boxed{D_{\rm qp}(E)=\sum_{\pm}g(\epsilon_F+\xi_\pm)
\left|\frac{d\xi_\pm}{dE}\right|
=\frac{2g(\epsilon_F)E}{\sqrt{E^2-\Delta^2}}.}
$$

Already at $\Delta=0$, folding $\xi$ into $|\xi|$ doubles the positive-axis density. Thus the printed formula is not the unweighted count of all states under the literal mapping without an additional normalization convention.

There is also a standard physical quantity with exactly the printed normalization: the [BCS electronic density of states](../../../../bcs-electronic-density-of-states.md), measured for example by [single-electron superconducting tunneling](../../../../single-electron-superconducting-tunneling.md). At positive $E$, the electron spectral weights of the two roots are the [BCS coherence factors](../../../../bcs-coherence-factors.md) $u_\pm^2=(1+\xi_\pm/E)/2$. They sum to one, so the weighted sum is $g(\epsilon_F)E/\sqrt{E^2-\Delta^2}$. This supplies a valid electronic-DOS interpretation, while keeping it distinct from counting every positive-[energy](../../../../energy-split.md) excitation. Spin degeneracy must be included consistently in $g$ and the transformed density; it does not remove the branch-counting issue.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
