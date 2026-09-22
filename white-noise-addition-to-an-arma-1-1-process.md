<h1 id="white-noise-addition-to-an-arma-1-1-process">White-noise addition to an ARMA(1,1) process</h1>

↑ **Parent:** [Autoregressive moving-average model](autoregressive-moving-average-model.md)

Adding [independent](independent-random-variables.md) [white noise](white-noise.md) of variance $w$ to a process with transfer function $(1+\theta z)/(1-\phi z)$ and driving variance $v$ gives numerator $A+2C\cos\omega$ in its rational [time-series spectral density](spectral-density-of-a-stationary-process.md). Put $P=A+2C$ and $Q=A-2C$. If both are positive, the invertible moving-average factor has coefficient $\alpha=(\sqrt P-\sqrt Q)/(\sqrt P+\sqrt Q)$ and driving variance $\lambda=(\sqrt P+\sqrt Q)^2/4$. Filtering the actual sum by $(1+\alpha B)^{-1}(1-\phi B)$ produces its [weak white noise](weak-white-noise.md) driver.

## ↑ Ancestors (6)

1. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/2/solution.md)
