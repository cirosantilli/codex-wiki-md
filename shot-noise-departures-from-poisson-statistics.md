# Shot noise departures from Poisson statistics

↑ **Parent:** [Shot noise](shot-noise.md)

The [Fano factor](fano-factor.md) $F_T$ compares count [variance](variance-split.md) with its mean over a specified gate. For a stationary unidirectional stream with fixed charge $q$, finite count second moments, and a generalized [autocovariance](autocovariance.md) with finite integral so that the long-gate limit exists,

$$
F_\infty=\lim_{T\to\infty}\frac{\operatorname{Var}(N_T)}{\mathbb E[N_T]},\qquad
S_I^{(1)}(0^+)=2qIF_\infty.
$$

The zero-[frequency](frequency.md) relation concerns the continuous fluctuation spectrum, excluding the mean spectral line. It follows by writing $\operatorname{Var}(Q_T)$ as the double integral of the current [autocovariance](autocovariance.md); for long $T$, its leading term is $T S_I^{(2)}(0)$. A finite-gate $F_T$, a frequency-dependent ratio $S_I^{(1)}(f)/(2qI)$, and a factor inferred from one filtered [variance](variance-split.md) are not interchangeable. The last is weighted by the instrument's $|K(f)|^2$.

Two original counting counterexamples show why [electric charge](electric-charge-split.md) discreteness is insufficient. In $n$ independent time slots, transfer one charge with [probability](probability.md) $p$ in each slot: the [binomial distribution](binomial-distribution.md) gives mean $np$, [variance](variance-split.md) $np(1-p)$ and [Fano factor](fano-factor.md) $1-p$. A random common origin for the slots removes a preferred time origin; the long-gate factor remains $1-p$. Alternatively, if independent [Poisson process](poisson-process-split.md) bursts each transfer exactly two charges, then $N_T=2M_T$ gives $\operatorname{Var}(N_T)=2\mathbb E[N_T]$ and factor $2$. Both count individual charges; only the first model allows at most one per slot, and the second groups them in pairs.

Consequently $2qI$ is a reference for independent unidirectional arrivals, not a universal noise law for all [electrical conductors](electrical-conductor.md). Correlations, charge multiplication, and bidirectional transfer require a more specific model. For example, independent opposite streams with positive current magnitudes $I_+$ and $I_-$ have net mean $I=I_+-I_-$ but one-sided fluctuation spectrum $2q(I_++I_-)$. Using $2q|I|$ would miss their fluctuations when the net current is small. At [thermal equilibrium](thermal-equilibrium-split.md), the full transport model must also respect [thermal electrical noise](thermal-electrical-noise.md); adding unrelated phenomenological formulas can double count the same underlying transfers.

## ↑ Ancestors (6)

1. [Shot noise](shot-noise.md)
2. [Noise (signal processing)](noise-signal-processing.md)
3. [Signal](signal.md)
4. [Signal processing](signal-processing.md)
5. [Electrical engineering](electrical-engineering-split.md)
6. [Codex Wiki](split.md)
