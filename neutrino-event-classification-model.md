# Neutrino event classification model

↑ **Parent:** [Lederman-Schwartz-Steinberger two-neutrino beam experiment](lederman-schwartz-steinberger-two-neutrino-beam-experiment.md)

How can the relative abundance of tracks and showers distinguish hypotheses? Consider an original teaching model, **with chosen inputs throughout**. Condition on a sample of $N$ selected events, each assigned exactly one of two labels: track or shower. Multitrack events and unclassified events lie outside this model. A shower label need not identify an [electron](electron.md); background can imitate it. Conversely, a true [electron](electron.md) interaction need not receive a shower label.

Let $b$ be the background fraction among selected events. Among the selected signal events, let $f$ be the fraction whose associated [charged lepton](charged-lepton.md) is an [electron](electron.md), with the remainder associated with a [muon](muon.md). These are fractions after event selection, rather than fractions of the incident [neutrino](neutrino.md) [particle flux](particle-flux.md). Define the [conditional probabilities](conditional-probability.md)

$$
a=\Pr(\mathrm{shower}\mid e,\mathrm{signal}),\qquad
r=\Pr(\mathrm{shower}\mid\mu,\mathrm{signal}),\qquad
q_b=\Pr(\mathrm{shower}\mid\mathrm{background}).
$$

Here $a$ and $r$ describe classification within the selected sample. They are not measured historical [detection efficiencies](detection-efficiency.md). The [law of total probability](law-of-total-probability.md) gives the overall shower [probability](probability.md)

$$
q(f,b)=(1-b)\bigl[af+r(1-f)\bigr]+bq_b.
$$

This formula is the bridge between an interaction hypothesis and a visible label. It keeps beam contamination, background and mistaken classification conceptually distinct: genuine [electron neutrino](electron-neutrino.md) interactions belong in $f$, while non-signal events belong in $b$.

Assume [independent random variables](independent-random-variables.md) for the event labels, all with this same $q$. If $K$ counts shower labels, every specified pattern with $k$ showers has [probability](probability.md) $q^k(1-q)^{N-k}$. Counting those patterns with a [binomial coefficient](binomial-coefficient-split.md) yields the [binomial distribution](binomial-distribution.md)

$$
\Pr(K=k)=\binom Nk q^k(1-q)^{N-k},\qquad
\mathbb E[K]=Nq,\qquad \operatorname{Var}(K)=Nq(1-q).
$$

The track count is $N-K$, so its [expected value](expected-value-split.md) is $N(1-q)$. At fixed $N$, the two counts cannot fluctuate independently. The [variance](variance-split.md) above measures sampling fluctuations under the stipulated model, not uncertainty in $a$, $r$, $b$ or $q_b$.

Choose $N=40$, $a=0.90$, $r=0.05$, $b=0.10$ and $q_b=0.40$. Compare a signal with only [muon](muon.md)-associated interactions ($f=0$) against one with equal selected [electron](electron.md)- and [muon](muon.md)-associated interactions ($f=1/2$). These give $q=0.085$ and $q=0.4675$, respectively. Their expected shower counts are $3.4$ and $18.7$; their expected track counts are $36.6$ and $21.3$. A background-only model with the specified $q_b$ gives $16$ showers and $24$ tracks on average. These are expectations, so they need not be integers.

<a id="image-chosen-binomial-distribution-model-expected-track-and-shower-counts-with-the-shower-count-distributions"></a>
![](neutrino-track-shower-classification-model.png)

**[Figure 4](#image-chosen-binomial-distribution-model-expected-track-and-shower-counts-with-the-shower-count-distributions). Chosen binomial distribution model: expected track and shower counts, with the shower-count distributions**. Original calculations for forty selected events and the stipulated classification and background probabilities. No historical counts, fitted efficiencies or reconstructed significance are plotted.

For a hypothetical observation $K=4$, the [likelihood ratio](likelihood-ratio.md) of the two signal models is

$$
\frac{\mathcal L(f=0)}{\mathcal L(f=1/2)}
=\left(\frac{0.085}{0.4675}\right)^4
\left(\frac{0.915}{0.5325}\right)^{36}
\simeq3.18\times10^5.
$$

The [binomial coefficient](binomial-coefficient-split.md) cancels because the same hypothetical sample is used in both [likelihoods](likelihood-function.md). This ratio is not the [probability](probability.md) that either hypothesis is true. A separate original check gives $\Pr(K\leq5)\simeq0.880$, $4.57\times10^{-6}$ and $1.44\times10^{-4}$ for the muon-associated, equal-mixture and specified background-only models, respectively.

Why are the controls essential? If the background-only model may choose any $q_b$, taking $q_b=K/N$ can fit the observed shower fraction. Counts alone then fail to distinguish it from a signal model. Independent background measurements and calibrated [particle identification](particle-identification.md) constrain that freedom. Changing the decay path additionally tests where the candidate-producing [particles](particle-physics.md) originate. The power of the experiment comes from combining apparatus interventions with event classification; the small [binomial distribution](binomial-distribution.md) model isolates only the latter part of that reasoning.

## ↑ Ancestors (5)

1. [Lederman-Schwartz-Steinberger two-neutrino beam experiment](lederman-schwartz-steinberger-two-neutrino-beam-experiment.md)
2. [Particle detector](particle-detector.md)
3. [Particle detection](particle-detection-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
