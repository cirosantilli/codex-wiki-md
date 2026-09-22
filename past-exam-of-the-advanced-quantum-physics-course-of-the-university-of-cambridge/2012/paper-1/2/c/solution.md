<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [three-level laser](../../../../../three-level-laser.md) uses a pump transition from ground level1 to a higher level3, rapid relaxation $3\to2$, and a long-lived upper lasing level2. The laser transition is $2\to1$, so its lower level is the ground state. Fast feeding and slow upper-state decay allow excitation to accumulate, unlike steady resonant pumping of a simple two-level transition.

[Stimulated emission](../../../../../stimulated-emission.md) adds photons to the stimulating optical mode, but ground-state [photon absorption](../../../../../photon-absorption.md) competes with it. The [population inversion](../../../../../population-inversion.md) condition is $N_2/g_2>N_1/g_1$ when the relevant transition strengths obey the usual Einstein relations. For equal degeneracies and negligible $N_3$, it reduces to **$N_2>N_1$, requiring more than half the active population in level2**.

For a simple pump rate R per ground-state emitter, fast $3\to2$ relaxation and negligible laser intensity, the [three-level laser rate equation](../../../../../three-level-laser-rate-equation.md) reduces to

$$
\dot N_2=RN_1-\frac{N_2}{\tau_{21}},\qquad N_1+N_2\simeq N_{\rm tot},\qquad
\boxed{\frac{N_2}{N_1}=R\tau_{21},\quad R\tau_{21}>1\ \text{for inversion}.}
$$

This [three-level ground-state inversion threshold](../../../../../three-level-ground-state-inversion-threshold.md) is only transparency; positive gain must also overcome optical losses. For an illustrative uniformly filled cavity of length $\ell$, equal absorption/emission cross-section $\sigma$, internal intensity-loss coefficient $\alpha_i$ and mirror power reflectivities $R_1,R_2$, the threshold condition is

$$
\boxed{g=\sigma(n_2-n_1)\geq\alpha_i+\frac1{2\ell}\ln\frac1{R_1R_2}.}
$$

Here $n_i$ are number densities, unlike the total populations $N_i$. The [optical resonator](../../../../../optical-cavity.md) supplies feedback and selects modes; a partially transmitting mirror couples out light. Spontaneous emission seeds the field, and stimulated transitions deplete the inversion until saturated gain balances loss. A [ruby laser](../../../../../ruby-laser.md) is the standard example. Real level degeneracies, branching losses and pump saturation modify the simple equations. [Chapter7§§7.1–7.2.1, printed pp.293–298, optical feedback and three-/four-level media; original reduced ground-state model specified above](../../../../../fundamentals-of-photonics-and-quantum-electronics-lecture-notes-by-franz-x-kartner.md)

<a id="2/c/image-original-three-level-laser-scheme-with-fast-feeding-of-a-metastable-upper-laser-state"></a>
![](../../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2012/paper-1-aqp2012-three-level-laser.png)

**[Figure 3](#2/c/image-original-three-level-laser-scheme-with-fast-feeding-of-a-metastable-upper-laser-state). Original three-level laser scheme with fast feeding of a metastable upper laser state**. [Source](paper-1-aqp2012-three-level-laser.py).

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../../split.md)
6. [Advanced Quantum Physics course of the University of Cambridge](../../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
