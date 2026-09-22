<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

First prove the [strong law for Brownian motion](../../../../../../strong-law-for-brownian-motion.md), $B_t/t\to0$ with probability one. For each $\varepsilon>0$, the [Gaussian tail bound](../../../../../../gaussian-tail-bound.md) gives

$$
\mathbb P(|B_n|>\varepsilon n)\leq2e^{-\varepsilon^2n/2}.
$$

By stationary increments and the [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md), followed by the same tail bound,

$$
\mathbb P\left(\sup_{0\leq s\leq1}|B_{n+s}-B_n|>\varepsilon n\right)
\leq4e^{-\varepsilon^2n^2/2}.
$$

Both bounds are summable in $n$. The [First Borel-Cantelli lemma](../../../../../../borel-cantelli-first-lemma.md) therefore implies that, eventually, both quantities inside these probability events are at most $\varepsilon n$. For $n\leq t\leq n+1$ this gives $|B_t|/t\leq2\varepsilon$. Intersect over a sequence of positive rational $\varepsilon$ tending to zero to obtain the asserted continuous-time limit.

On this one [almost sure event](../../../../../../almost-sure-event.md),

$$
\frac{B_t+at}{t}\longrightarrow a,
$$

so $B_t+at\to+\infty$ for $a>0$ and to $-\infty$ for $a<0$. For each real $x$, the path is eventually strictly on the corresponding side of $x$. Hence

$$
\boxed{\{t\geq0:B_t+at=x\}\text{ is bounded for every }x\in\mathbb R.}
$$

The same event works simultaneously for all levels $x$, giving the requested transience of [Brownian motion with drift](../../../../../../brownian-motion-with-drift.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
