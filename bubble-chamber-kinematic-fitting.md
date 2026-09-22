# Bubble-chamber kinematic fitting

↑ **Parent:** [Alvarez hydrogen-bubble-chamber reconstruction and resonances](alvarez-hydrogen-bubble-chamber-reconstruction-and-resonances.md)

Alvarez describes a progression from measured coordinates to [momenta](momentum-split.md) and angles, then conservation-constrained fits testing alternative track identities. Computer programs made the repeated tests practical; an insufficiently constrained event could retain several hypotheses.[UCRL-18696, printed pp. 30–33: HYDRO, PANG, GUTS, KICK and SUMX](recent-developments-in-particle-physics-by-luis-walter-alvarez.md)

A mathematical formulation explains what such a fit can establish. Let $y$ collect measured [momenta](momentum-split.md) and angles, with positive-definite [covariance matrix](covariance-matrix.md) $V$. For a chosen reaction hypothesis, adjust them to $x$ by minimizing a [generalized least squares](generalized-least-squares.md) objective,

$$
\chi^2=(x-y)^{\mathsf T}V^{-1}(x-y),\qquad g(x)=0.
$$

The constraints $g$ express [four-momentum conservation](four-momentum-conservation.md) and any independently known daughter [masses](mass.md). For each proposed identity, calculate [energy](energy-split.md) from the [energy–momentum relation](energy-momentum-relation.md), $E_i^2=m_i^2c^4+c^2|\mathbf p_i|^2$. A missing [neutral particle](neutral-particle.md) adds unknowns; a measured decay vertex can add geometric constraints. Compatibility depends on the measurement errors and the independent constraints, not just the smallest raw $\chi^2$ among unrelated fits.

A simple independent check uses a single [momentum conservation](momentum-conservation.md) constraint. Suppose two measured one-dimensional [momenta](momentum-split.md) are $0.32$ and $-0.28\,\mathrm{GeV}/c$, each with independent [standard deviation](standard-deviation.md) $0.02\,\mathrm{GeV}/c$, and a stipulated parent at rest requires their sum to vanish. Minimizing the two equal-weight squared changes gives fitted values $0.30$ and $-0.30\,\mathrm{GeV}/c$, with $\chi^2=2$. A fit repairs a mismatch according to a hypothesis; it does not prove that hypothesis. This one-component illustration is not a complete reaction fit.

## ↑ Ancestors (7)

1. [Alvarez hydrogen-bubble-chamber reconstruction and resonances](alvarez-hydrogen-bubble-chamber-reconstruction-and-resonances.md)
2. [Hydrogen bubble chamber](hydrogen-bubble-chamber.md)
3. [Bubble chamber](bubble-chamber.md)
4. [Particle detector](particle-detector.md)
5. [Particle detection](particle-detection-split.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Invariant-mass selection of bubble-chamber events](invariant-mass-selection-of-bubble-chamber-events.md)
