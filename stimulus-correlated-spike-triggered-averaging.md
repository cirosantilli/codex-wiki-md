# Stimulus-correlated spike-triggered averaging

↑ **Parent:** [Spike-triggered average](spike-triggered-average.md)

For a single linear filter followed by a rate nonlinearity and a Gaussian stimulus-history vector $s$ with covariance $C$, Gaussian integration by parts gives $\mathbb E[s\,g(k^Ts)]\propto Ck$. Thus a [spike-triggered average](spike-triggered-average.md) estimates $Ck$, rather than $k$ directly, when the stimulus is correlated. Covariance correction, with regularization if necessary, can recover the filter direction. For an even nonlinearity the proportionality factor can vanish; then a one-filter average is insufficient.

## ↑ Ancestors (5)

1. [Spike-triggered average](spike-triggered-average.md)
2. [Computational neuroscience](computational-neuroscience.md)
3. [Neuroscience](neuroscience.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/4/a/solution.md)
