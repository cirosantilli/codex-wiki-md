<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

There are four relevant [tree-level Feynman diagrams](../../../../tree-level-feynman-diagram.md): $s$-channel [photon](../../../../photon.md), [Z boson](../../../../z-boson.md) and [Higgs boson](../../../../higgs-boson.md) exchange, and $t$-channel electron-neutrino exchange. The [electron](../../../../electron.md) and [Positron](../../../../positron.md) are incoming, and $W^-$ and $W^+$ outgoing. The Higgs diagram is normally tiny because its electron coupling is proportional to $m_e$; it should nevertheless be included in the requested list.

<a id="3/image-the-four-tree-level-diagrams-for-electron-positron-annihilation-into-a-charged-w-pair"></a>
![](../../../../past-exam-of-the-gauge-field-theory-course-of-the-university-of-cambridge/2016/paper-1-w-pair-diagrams.png)

**[Figure 1](#3/image-the-four-tree-level-diagrams-for-electron-positron-annihilation-into-a-charged-w-pair). The four tree-level diagrams for electron–positron annihilation into a charged W pair**. Original schematics. Fermion arrows show particle-number flow, which opposes the momentum of an incoming positron. W lines are labelled by charge.

Let $v=2m_W/g$. The [Higgs-electron coupling](../../../../higgs-electron-coupling.md) is $m_e/v$, while the [Higgs boson coupling to W bosons](../../../../higgs-boson-coupling-to-w-bosons.md) is $2m_W^2g_{\mu\nu}/v$. Multiplying the vertices and scalar propagator gives, up to an irrelevant overall phase,

$$
\mathcal M_h=\frac{g^2m_e}{2(s-m_h^2)}\bar v(p_2)u(p_1)\,\epsilon_1^*\cdot\epsilon_2^*.
$$

A scalar propagator has no vector index, the [Yukawa interaction](../../../../yukawa-interaction.md) supplies the scalar spinor bilinear, and the second vertex contracts the two polarization vectors. We retain the tree propagator and neglect widths, consistently with the stated leading-order calculation.

For unpolarized incoming beams the [spin average](../../../../spin-average.md) is $1/4$, not a sum without normalization. The [fermion spin sums](../../../../fermion-spin-sum.md) and [gamma-matrix trace](../../../../gamma-matrix-trace.md) identities give

$$
\begin{aligned}
\frac14\sum_{r,t}|\bar v_t(p_2)u_r(p_1)|^2
&=\frac14\operatorname{tr}\left[(\not p_2-m_e)(\not p_1+m_e)\right]\\
&=p_1\cdot p_2-m_e^2
=\frac{s-4m_e^2}{2}.
\end{aligned}
$$

The terms with one gamma matrix have zero trace; the two-gamma trace gives $4p_1\cdot p_2$. Both final polarization states are specified as longitudinal, so no final polarization average is appropriate.

In the [centre-of-momentum frame](../../../../center-of-momentum-frame.md), take $k_1=(E,k\widehat{\mathbf n})$ and $k_2=(E,-k\widehat{\mathbf n})$, where $E=\sqrt s/2$ and $k^2=E^2-m_W^2$. A pair of [longitudinal polarization vectors](../../../../longitudinal-polarization-vector.md) is

$$
\epsilon_{1L}=\frac1{m_W}(k,E\widehat{\mathbf n}),\qquad
\epsilon_{2L}=\frac1{m_W}(k,-E\widehat{\mathbf n}).
$$

Each obeys $\epsilon_i\cdot k_i=0$ and $\epsilon_i^2=-1$. Their contraction is angle independent:

$$
\epsilon_{1L}\cdot\epsilon_{2L}=\frac{k^2+E^2}{m_W^2}=\frac{s}{2m_W^2}-1.
$$

Consequently

$$
\boxed{\overline{|\mathcal M_h|^2}_{LL}=\frac{g^4m_e^2(s-4m_e^2)}{8(s-m_h^2)^2}\left(\frac{s}{2m_W^2}-1\right)^2.}
$$

For the [two-body scattering cross section](../../../../two-body-scattering-cross-section.md), the outgoing-to-incoming momentum ratio is

$$
\frac{k}{p}=\frac{\beta_W}{\beta_e},\qquad
\beta_W=\sqrt{1-\frac{4m_W^2}{s}},\quad
\beta_e=\sqrt{1-\frac{4m_e^2}{s}}.
$$

The source's final sentence interchanges the particle names attached to these two momenta; physical final-state phase space and initial-state flux fix the ratio as written here. Since the Higgs-only spin-averaged expression is isotropic, integrating the [solid angle](../../../../solid-angle.md) gives $4\pi$:

$$
\begin{aligned}
\sigma_{h,LL}
&=\frac1{16\pi s}\frac{\beta_W}{\beta_e}\overline{|\mathcal M_h|^2}_{LL}\\
&=\boxed{\frac{g^4m_e^2\beta_e\beta_W}{128\pi(s-m_h^2)^2}\left(\frac{s}{2m_W^2}-1\right)^2},\qquad s\ge4m_W^2.
\end{aligned}
$$

There is no identical-particle factor: $W^+$ and $W^-$ are distinguishable. The threshold factor $\beta_W$ makes this contribution vanish when the outgoing momentum vanishes. This is the isolated squared Higgs amplitude for a specified longitudinal pair, not the complete physical cross section: the full result squares the coherent sum of all four amplitudes and includes their interference.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2016](../../split.md)
4. [Past exam of the gauge field theory course of the University of Cambridge](../../../split.md)
5. [Gauge Field Theory course of the University of Cambridge](../../../../gauge-field-theory-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
