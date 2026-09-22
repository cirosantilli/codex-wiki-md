# Orientation tuning curve

↑ **Parent:** [Orientation selectivity](orientation-selectivity.md)

An [orientation tuning curve](orientation-tuning-curve.md) plots a specified response against the stimulus-axis [angle](angle.md) $\theta$, with the other stimulus variables controlled. A practical count summary for [extracellular single-unit recording](extracellular-single-unit-recording.md) is

$$
\widehat r(\theta)=\frac{1}{mT}\sum_{k=1}^{m}N_k(\theta),
$$

where $N_k(\theta)$ counts [action potentials](action-potential.md) in the same duration $T>0$ on trial $k$, and $m$ is the number of repeats at each [angle](angle.md). This estimates spikes per unit time in that window; the window must specify whether it covers onset, sustained stimulation, or both. Record a blank-background response separately, and report whether it has been subtracted. Randomizing [angle](angle.md) order and repeating each condition helps separate [orientation selectivity](orientation-selectivity.md) from changes over time, including [neural adaptation](neural-adaptation.md). This is a proposed measurement procedure, not a claim that the original experiments used this estimator.

A [simple cell](simple-cell.md)'s [orientation tuning curve](orientation-tuning-curve.md) can also change when the stimulus shifts. An [angle](angle.md) sweep at fixed [phase](phase-waves.md), a sweep averaging over [phase](phase-waves.md), and a sweep of moving stripes ask different questions. Consequently, a single preferred [angle](angle.md) does not specify the whole [receptive field](receptive-field.md). The toy curve under [orientation selectivity](orientation-selectivity.md) holds [phase](phase-waves.md) fixed and plots dimensionless output, rather than spikes per second.

## ↑ Ancestors (5)

1. [Orientation selectivity](orientation-selectivity.md)
2. [Primary visual cortex](primary-visual-cortex.md)
3. [Neuroscience](neuroscience-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Gabor filter](gabor-filter.md)
- [Orientation selectivity](orientation-selectivity.md)
- [Orientation tuning curve](orientation-tuning-curve.md)
