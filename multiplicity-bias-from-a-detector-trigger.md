# Multiplicity bias from a detector trigger

↑ **Parent:** [Trigger (particle physics)](trigger-particle-physics.md)

A trigger changes which particle populations are common in the recorded sample. Let $N$ be the number of particles in an event, and stipulate an independent [Bernoulli distribution](bernoulli-distribution.md) for each particle's ability to produce an accepted telescope signal, with success [probability](probability.md) $\epsilon$. If any successful particle suffices, the event acceptance is

$$
A(n)=1-(1-\epsilon)^n.
$$

This is a deliberately simplified model. Its $\epsilon$ includes the joint geometrical acceptance and response of the whole telescope; it is not an assumed universal single-counter efficiency. Actual shower directions, spatial correlations and shared electronics can violate the independence assumption.

The [conditional probability](conditional-probability.md) formula gives

$$
\Pr(N=n\mid\mathrm{trigger})=
\frac{A(n)\Pr(N=n)}{\sum_m A(m)\Pr(N=m)}.
$$

For chosen underlying fractions $\Pr(N=1)=0.90$, $\Pr(N=5)=0.10$ and $\epsilon=0.15$, the two acceptances are $0.15$ and $0.5563$. Five-particle events consequently form about $29.18\%$ of recorded events. **A population that is only $10\%$ of incoming events can occupy nearly $30\%$ of the photographs.** This is [selection bias](selection-bias.md), not evidence that the source population changed.

<a id="image-a-coincidence-window-trades-timing-acceptance-against-background-while-a-trigger-enriches-events-with-more-particles"></a>
![](coincidence-window-and-shower-selection.png)

**[Figure 9](#image-a-coincidence-window-trades-timing-acceptance-against-background-while-a-trigger-enriches-events-with-more-particles). A coincidence window trades timing acceptance against background, while a trigger enriches events with more particles**. Original calculations with the explicitly chosen rates, Gaussian timing spread and independent-particle acceptance model in the text. No historical event counts or measured timing curves are reproduced.

## ↑ Ancestors (5)

1. [Trigger (particle physics)](trigger-particle-physics.md)
2. [Particle detector](particle-detector.md)
3. [Particle detection](particle-detection-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Blackett-Occhialini triggered cloud-chamber experiment](blackett-occhialini-triggered-cloud-chamber-experiment.md)
- [Detector dead time](detector-dead-time.md)
