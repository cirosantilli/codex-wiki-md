# Biased-step entropy production model

↑ **Parent:** [Fluctuation theorem](fluctuation-theorem.md)

Take $n$ [independent](independent-random-variables.md) steps, each $+1$ with [probability](probability.md) $p>1/2$ and $-1$ with [probability](probability.md) $q=1-p>0$. Reverse a step sequence by reading it backward and changing each sign; use the same biased law for both experiments. With $K$ positive steps, the forward sequence weight is $p^Kq^{n-K}$ and its reversed weight is $p^{n-K}q^K$. Their [logarithm](logarithm.md) ratio is

$$
S_n=(2K-n)a,\qquad a=\ln(p/q)>0,\qquad
K\sim\operatorname{Binomial}(n,p).
$$

Here $S_n$ is dimensionless [entropy production](entropy-production.md), not an [entropy](entropy.md) in joules per kelvin. A [Markov chain](markov-chain.md) on a three-state ring gives a state-space realization: start uniformly, take a clockwise step with [probability](probability.md) $p$ and a counterclockwise step with [probability](probability.md) $q$. The uniform [stationary distribution](stationary-distribution.md) makes endpoint weights cancel. A physical interpretation as exchanged [heat](heat.md) requires [local detailed balance](local-detailed-balance.md) with bath [entropy](entropy.md) $\pm k_Ba$ per directed step; the abstract model alone specifies path [probabilities](probability.md).

For an allowed value $s=a(2k-n)$, the [binomial distribution](binomial-distribution.md) gives

$$
p_n(s)=\binom nkp^kq^{n-k},\qquad
\frac{p_n(s)}{p_n(-s)}
=\frac{\binom nkp^kq^{n-k}}{\binom n{n-k}p^{n-k}q^k}
=\left(\frac pq\right)^{2k-n}=e^s.
$$

This is an exact same-law finite [fluctuation theorem](fluctuation-theorem.md), with no long-time approximation. For $p=3/4$, $n=9$ and $k=6$, $s=3\ln3$ and $p_n(s)/p_n(-s)=27$. The positive mean is $\langle S_n\rangle=na(p-q)$, although the all-negative path has nonzero [probability](probability.md) $q^n$. Directly, $\langle e^{-S_n}\rangle=(pe^{-a}+qe^a)^n=(q+p)^n=1$.

<a id="image-exact-biased-step-model-discrete-entropy-production-probabilities-and-their-log-ratio-at-nine-steps"></a>
![](biased-step-entropy-probabilities.png)

**[Figure 17](#image-exact-biased-step-model-discrete-entropy-production-probabilities-and-their-log-ratio-at-nine-steps). Exact biased-step model: discrete entropy-production probabilities and their log ratio at nine steps**.

The left panel shows exact [probability masses](probability-mass.md) for $p=3/4$, with negative values highlighted; the right panel tests the [logarithm](logarithm.md) ratio against $s$. These are model values, without experimental measurements or simulated measurement noise.

**Table of contents**

- [Negative entropy production over finite durations](negative-entropy-production-over-finite-durations.md)

## ↑ Ancestors (8)

1. [Fluctuation theorem](fluctuation-theorem.md)
2. [Entropy production](entropy-production.md)
3. [Stochastic thermodynamics](stochastic-thermodynamics.md)
4. [Thermodynamics](thermodynamics-split.md)
5. [Statistical physics](statistical-physics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Fluctuation theorem](fluctuation-theorem.md)
