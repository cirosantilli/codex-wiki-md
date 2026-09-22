<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $p_{rs}(t)=P(X(u+t)=s\mid X(u)=r)$ and $P(t)=e^{Qt}$, where time homogeneity removes dependence on $u$. A recorded state at the next clinic visit contributes a [transition probability](../../../../../../transition-probability.md); an exactly observed death contributes a [statistical probability density](../../../../../../probability-density-function.md), not the [probability](../../../../../../probability.md) of being dead at that time. If the last recorded living state is $r$, the [mixed panel and exact-death likelihood](../../../../../../mixed-panel-and-exact-death-likelihood.md) factor after an interval $t$ is

$$
g_{r3}(t)=\sum_{j=1}^2p_{rj}(t)q_{j3}=\frac{d}{dt}p_{r3}(t).
$$

This sums over the unobserved living state immediately before death.

Conditioning on the recorded initial states, the contribution of the three displayed patient histories is

$$
\boxed{L(Q)=p_{11}(8.5)\,p_{11}(26.3)\,p_{22}(12.6)\left[p_{21}(34.6)q_{13}+p_{22}(34.6)q_{23}\right].}
$$

In this irreversible [illness-death model](../../../../../../illness-death-model.md), $p_{21}=0$, $p_{11}(t)=e^{-(a+b)t}$ and $p_{22}(t)=e^{-ct}$, simplifying it to

$$
\boxed{L(Q)=c\exp\{-34.8(a+b)-47.2c\}.}
$$

The factor $c$ is essential: the death time is known exactly. Replacing the final [statistical probability density](../../../../../../probability-density-function.md) by $p_{23}(34.6)$ would instead model interval observation of death and give a different [likelihood](../../../../../../likelihood-function.md).

The assumptions are independent patient histories with common rates; the Markov property; constant rates over calendar/follow-up time in this model; the stated absence of recovery and absorption at death; accurate state labels and death times; and an observation/follow-up mechanism that is noninformative for the latent process given the observed history. Clinic dates are conditioned on. The displayed living endpoints contribute only the shown observations, with noninformative [right censoring](../../../../../../right-censoring.md) if they are follow-up endpoints. Initial state [probabilities](../../../../../../probability.md) are omitted by conditioning on them. Progression between visits can be unobserved, which is precisely why [panel-observed multi-state likelihood](../../../../../../panel-observed-multi-state-likelihood.md) uses the [matrix exponential](../../../../../../matrix-exponential.md) rather than assuming a transition occurs at a visit.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
