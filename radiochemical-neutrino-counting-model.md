# Radiochemical neutrino counting model

↑ **Parent:** [Homestake experiment](homestake-experiment.md)

An idealized [radiochemical neutrino counting model](radiochemical-neutrino-counting-model.md) separates production, survival, recovery and readout. Suppose a freshly cleared target produces atoms at a constant rate $R$ during exposure $T$. Each atom has [nuclear decay constant](nuclear-decay-constant.md) $\lambda=\log 2/h$, where $h$ is its [half-life](half-life.md). The expected surviving population obeys

$$
\frac{dN}{dt}=R-\lambda N,\qquad N(0)=0,\qquad N(T)=\frac R\lambda(1-e^{-\lambda T}).
$$

The proof is to multiply the [differential equation](differential-equation-split.md) by $e^{\lambda t}$ and apply [integration](integral-split.md). The expression also follows by summing the [exponential decay](exponential-decay.md) survival probabilities of atoms produced at every earlier time. Production does not imply eventual recovery: atoms can decay during exposure.

Let $\eta$ be the fraction recovered instantaneously at extraction, $d$ the subsequent delay before counting, $\epsilon$ the probability of recording a decay, and $W$ the counting duration. The expected signal pulses are

$$
\mu_s=\epsilon\eta N(T)e^{-\lambda d}(1-e^{-\lambda W}).
$$

With constant background rate $b$, the expected total is $\mu=\mu_s+bW$. During counting, the expected instantaneous pulse rate is $s(t)+b$, with $s(t)=\epsilon\eta\lambda N(T)e^{-\lambda(d+t)}$. Equal time windows therefore lose signal by the factor $e^{-\lambda\Delta t}$ while a constant background stays unchanged. Fitting the time dependence helps distinguish [radioactive decay](radioactive-decay.md) from that background; it does not recover individual capture times.

For an original worked example choose $Rh=20$, $T=W=h$, $d=0$, $\eta=0.8$, $\epsilon=0.5$ and $bh=0.2$. These are illustrative assumptions. Then $N(T)=10/\log 2$, and

$$
\mu_s=\frac2{\log 2}\simeq2.8854,\qquad\mu\simeq3.0854.
$$

Doubling the exposure does not double the surviving inventory: $N(2h)/N(h)=3/2$. A delay of one [half-life](half-life.md) halves the signal. At $\lambda T\ll1$, $N(T)\simeq RT$; at long exposure it saturates at $R/\lambda$. These limits explain why a large target and repeated extraction can matter more than simply waiting longer. The model neglects time-dependent production, finite extraction duration, residual atoms between runs and time-dependent backgrounds.

## ↑ Ancestors (10)

1. [Homestake experiment](homestake-experiment.md)
2. [Solar neutrino detection](solar-neutrino-detection.md)
3. [Solar neutrino](solar-neutrino.md)
4. [Sun](sun.md)
5. [Star](star.md)
6. [Stellar astrophysics](stellar-astrophysics-split.md)
7. [Astrophysics](astrophysics-split.md)
8. [Branches of physics](branches-of-physics.md)
9. [Physics](physics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Homestake experiment](homestake-experiment.md)
- [Radiochemical neutrino counting model](radiochemical-neutrino-counting-model.md)
