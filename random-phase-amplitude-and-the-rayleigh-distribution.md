# Random-phase amplitude and the Rayleigh distribution

↑ **Parent:** [Rayleigh distribution](rayleigh-distribution.md)

In an 1880 paper, [John William Strutt](john-william-strutt-3rd-baron-rayleigh.md), known as [Lord Rayleigh](john-william-strutt-3rd-baron-rayleigh.md), studied the resultant of many [oscillations](oscillation.md) with a common [frequency](frequency.md) and arbitrary [oscillation phases](phase-waves.md). His large-number calculation distinguished a mean intensity from a definite resultant [amplitude](wave-amplitude.md) and used planar coordinates followed by a polar integral. The resulting [amplitude](wave-amplitude.md) density is the [Rayleigh distribution](rayleigh-distribution.md) in a different scale convention. This is a large-number description, not an exact law for every finite collection of [oscillations](oscillation.md).[Philosophical Magazine, Series 5, volume 10 (August 1880), pp. 73–74: expected intensity versus definite resultant; pp. 75–77: planar construction and polar integration; primary-paper transcription inspected on Scribd](on-the-resultant-of-a-large-number-of-vibrations-of-the-same-pitch-and-of-arbitrary-phase-by-john-william-strutt-3rd-baron-rayleigh.md)

To see the connection in a chosen model, take [independent](independent-random-variables.md) [oscillation phases](phase-waves.md) $\Theta_j$ with [uniform distribution](continuous-uniform-distribution.md) on $[0,2\pi)$ and equal component [amplitude](wave-amplitude.md) $a$. The [phasor](phasor.md) sum has coordinates

$$
X_n=a\sum_{j=1}^n\cos\Theta_j,\qquad Y_n=a\sum_{j=1}^n\sin\Theta_j.
$$

Both have [mean](expected-value-split.md) zero, [variance](variance-split.md) $na^2/2$ and zero [covariance](covariance.md). The [multivariate central limit theorem](multivariate-central-limit-theorem.md) gives an approximately circular [Gaussian random vector](gaussian-random-vector.md) for large $n$, with $\sigma=a\sqrt{n/2}$. Its [amplitude](wave-amplitude.md) $\sqrt{X_n^2+Y_n^2}$ is therefore approximately Rayleigh. For every finite $n$, that [amplitude](wave-amplitude.md) is bounded by $na$, whereas a [Rayleigh distribution](rayleigh-distribution.md) has an unbounded tail. At $n=1$ it is exactly $a$. This simple endpoint check prevents the approximation from becoming a false exact identity.

## ↑ Ancestors (8)

1. [Rayleigh distribution](rayleigh-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
