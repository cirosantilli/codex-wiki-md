<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Treat the atmospheric [proton](../../../../proton.md) as stationary in the [Earth](../../../../earth.md) frame, the incident [antiproton](../../../../antiproton.md) as vertically downward, and neglect atmospheric [energy loss](../../../../energy-loss.md), scattering and the [Earth](../../../../earth.md)'s curvature initially. Take $m_pc^2=0.9383\,\mathrm{GeV}$. [Conservation of energy](../../../../conservation-of-energy.md) and equal outgoing [energies](../../../../energy-split.md) give

$$
E_\mu=\frac{35+0.9383}{2}\,\mathrm{GeV}=17.9692\,\mathrm{GeV},\qquad \gamma_\mu=\frac{E_\mu}{0.106\,\mathrm{GeV}}\simeq169.52.
$$

Equal [energies](../../../../energy-split.md) imply equal [momentum](../../../../momentum-split.md) magnitudes. Their transverse [momenta](../../../../momentum-split.md) cancel, so the two [muons](../../../../muon.md) have equal downward components $p_z=p_{\bar p}/2$, where

$$
p_{\bar p}c=\sqrt{(35\,\mathrm{GeV})^2-(0.9383\,\mathrm{GeV})^2}\simeq34.9874\,\mathrm{GeV}.
$$

Each [muon](../../../../muon.md) therefore makes an [angle](../../../../angle.md) $\theta$ with the downward vertical satisfying

$$
\cos\theta=\frac{p_{\bar p}c/2}{\sqrt{E_\mu^2-m_\mu^2c^4}}\simeq0.9735.
$$

The paths are not both vertical: replacing their path lengths by $20\,\mathrm{km}$ would miss this two-body kinematic correction. Since $v_z=p_zc^2/E_\mu$, the proper flight time over vertical height $H$ is

$$
\Delta\tau_\mu=\frac{H}{\gamma_\mu v_z}=\frac{2Hm_\mu c^2}{c(p_{\bar p}c)}.
$$

For [equal-energy atmospheric muon-pair survival](../../../../equal-energy-atmospheric-muon-pair-survival.md), independent exponential [particle decays](../../../../particle-decay.md) with mean proper [muon lifetime](../../../../muon-lifetime.md) $\tau_0=2.2\,\mu\mathrm s$, both survive with [probability](../../../../probability.md)

$$
\boxed{P_{\rm both}=\exp\left[-\frac{4Hm_\mu c^2}{c\tau_0(p_{\bar p}c)}\right]\simeq0.692.}
$$

Equivalently each travels about $20.55\,\mathrm{km}$, with proper flight time about $0.404\,\mu\mathrm s$, and survives with [probability](../../../../probability.md) about $0.832$. The result is decay-only survival to an ideal surface, not a prediction including air interactions or detector efficiency. For a spherical [Earth](../../../../earth.md) of radius $R_E$, the exact path length is $\ell=(R_E+H)\cos\theta-\sqrt{R_E^2-(R_E+H)^2\sin^2\theta}$; inserting $P_{\rm both}=\exp[-2\ell/(\gamma_\mu v_\mu\tau_0)]$ gives a small curvature correction.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
