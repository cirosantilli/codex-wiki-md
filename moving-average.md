# Moving average

↑ **Parent:** [Finite impulse response](finite-impulse-response.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Moving_average)

A moving average replaces each value by an average over a moving window of neighboring values. The simple trailing version with positive integer window length $M$ is the [causal filter](causal-filter.md)

$$
y[n]=\frac1M\sum_{j=0}^{M-1}x[n-j].
$$

It is a [finite impulse response](finite-impulse-response.md) [linear time-invariant system](linear-time-invariant-system.md). A constant [input](input-computer-science.md) remains unchanged because the weights sum to one. Weighted and centered averages are other choices; the definition of the window determines both the weights and whether future values are needed.

For an exact five-sample example, let

$$
x[n]=\sin(2\pi(0.025)n)+0.45\sin(2\pi(0.2)n),
$$

defined at every integer index. The first component completes one cycle in forty samples and the second in five. Averaging five consecutive samples cancels the second component exactly. The first becomes

$$
y[n]=A\sin(2\pi(0.025)(n-2)),\qquad
A=\frac{\sin(5\pi(0.025))}{5\sin(\pi(0.025))}\approx0.975498.
$$

The remaining component is slightly smaller and delayed by two samples; the filter does not recover the original component unchanged.

<a id="image-a-five-sample-moving-average-cancels-one-sinusoid-while-attenuating-and-delaying-another"></a>
![](moving-average-signal-delay.png)

**[Figure 22](#image-a-five-sample-moving-average-cancels-one-sinusoid-while-attenuating-and-delaying-another). A five-sample moving average cancels one sinusoid while attenuating and delaying another**.

The example is in steady operation: its early [output](output-computing.md) values use the specified negative-index samples. Starting a device at $n=0$ with an unknown past requires an initialization rule. Treating earlier samples as zero, shortening the initial window, and postponing output until a full window is available produce different initial values.

For zero-mean [uncorrelated random variables](uncorrelated-random-variables.md) $\varepsilon[n]$ with common [variance](variance-split.md) $\sigma^2$, the averaged disturbance has

$$
\operatorname{Var}\left(\frac1M\sum_{j=0}^{M-1}\varepsilon[n-j]\right)=\frac{\sigma^2}{M}.
$$

The [standard deviation](standard-deviation.md) decreases by $\sqrt M$, but successive filtered errors share samples and are generally correlated. This variance calculation also assumes the wanted component is not damaged by averaging. A rapidly changing feature can be suppressed along with the disturbance.

The [frequency response](frequency-response.md) explains the cancellation and limits of this method. A [moving average](moving-average.md) preserves low [frequencies](frequency.md) comparatively well, yet its side lobes make it a poor substitute for a sharply selective frequency cutoff. Smith develops this time-domain versus frequency-domain distinction in [The Scientist and Engineer's Guide to Digital Signal Processing, chapter 15: moving-average filters](https://www.dspguide.com/CH15.PDF).

## ↑ Ancestors (5)

1. [Finite impulse response](finite-impulse-response.md)
2. [Linear filter](linear-filter.md)
3. [Signal processing](signal-processing.md)
4. [Electrical engineering](electrical-engineering-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Causal filter](causal-filter.md)
- [Electrical engineering](electrical-engineering-split.md)
- [Finite impulse response](finite-impulse-response.md)
- [Frequency response](frequency-response.md)
- [Impulse response](impulse-response.md)
- [Linear filter](linear-filter.md)
- [Low-pass filter](low-pass-filter.md)
- [Moving average](moving-average.md)
- [Signal processing](signal-processing.md)
