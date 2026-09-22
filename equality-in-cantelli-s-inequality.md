<h1 id="equality-in-cantelli-s-inequality">Equality in Cantelli's inequality</h1>

↑ **Parent:** [Cantelli inequality](cantelli-inequality.md)

For $a>0$ and $\sigma^2>0$, place [probabilities](probability.md)

$$
\mathbb P(X=\mu+a)=\frac{\sigma^2}{\sigma^2+a^2},\qquad
\mathbb P\left(X=\mu-\frac{\sigma^2}{a}\right)=\frac{a^2}{\sigma^2+a^2}.
$$

Their weighted deviations cancel, giving [expected value](expected-value-split.md) $\mu$; their weighted squared deviations give [variance](variance-split.md) $\sigma^2$. Only the upper point belongs to $X-\mu\geq a$, so its [tail probability](tail-probability.md) attains [Cantelli's inequality](cantelli-inequality.md). With $a=2$, $\sigma^2=1$, $\mu=0$, the locations are two and $-1/2$, with masses $1/5$ and $4/5$. The optimized shift makes the lower point zero before squaring, explaining equality in the [Markov's inequality](markov-s-inequality.md) step.

The threshold convention matters: this example has $\mathbb P(X-\mu>a)=0$. For a strict threshold, placing the upper point at $a+\varepsilon$ instead gives probabilities approaching the same bound as $\varepsilon\downarrow0$, with the prescribed [mean](expected-value-split.md) and [variance](variance-split.md) retained. Extra restrictions on the [support of a probability distribution](support-of-a-probability-distribution.md) can change which extremal models are allowed.

## ↑ Ancestors (8)

1. [Cantelli inequality](cantelli-inequality.md)
2. [Chebyshev's inequality](chebyshev-s-inequality.md)
3. [Probability inequality](probability-inequality-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cantelli inequality](cantelli-inequality.md)
