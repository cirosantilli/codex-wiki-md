# Biased random walk

↑ **Parent:** [Simple random walk on the integer line](simple-random-walk-on-the-integer-line.md)

A biased random walk on the [integer](integer-split.md) line takes unit steps right and left with unequal [probabilities](probability.md) $p$ and $1-p$, using [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) as [increments](increment.md). For $S_0=0$, the [expected value](expected-value-split.md) is $n(2p-1)$: positive for $p>1/2$ and negative for $p<1/2$. Changing $p$ to $1-p$ reverses the preferred direction. The exact endpoint [probability mass function](probability-mass-function.md) is given under [simple random walk on the integer line](simple-random-walk-on-the-integer-line.md).

For example, with $p=0.65$ each step has [expected value](expected-value-split.md) $0.30$ and [variance](variance-split.md) $0.91$. After $80$ steps,

$$
\mathbb E S_{80}=24,\qquad \operatorname{Var}(S_{80})=72.8,\qquad
\sigma_{80}=\sqrt{72.8}\approx8.532.
$$

The displacement of the [expected value](expected-value-split.md) from zero is about $24/8.532\approx2.813$ [standard deviations](standard-deviation.md), yet individual [sample paths](sample-path.md) still move left as well as right, as the figure under [simple random walk](simple-random-walk.md) illustrates. Bias lets this elementary [stochastic process](stochastic-process-split.md) model an average directional tendency while retaining fluctuations. Boundary and return questions have their own treatments under [gambler's ruin](gambler-s-ruin.md) and the specialized children below.

**Table of contents**

- [Exponential martingale of a biased simple random walk](exponential-martingale-of-a-biased-simple-random-walk.md)
- [Hitting time of a downward-biased walk reflected at an upper barrier](hitting-time-of-a-downward-biased-walk-reflected-at-an-upper-barrier.md)
- [Diffusion limit of a weakly biased random walk](diffusion-limit-of-a-weakly-biased-random-walk.md)
- [Maximum of a downward-biased random walk](maximum-of-a-downward-biased-random-walk.md)
- [Reflected biased random walk on the nonnegative integers](reflected-biased-random-walk-on-the-nonnegative-integers.md)

## ↑ Ancestors (10)

1. [Simple random walk on the integer line](simple-random-walk-on-the-integer-line.md)
2. [Random walk on a graph](random-walk-on-a-graph.md)
3. [Random walk](random-walk-split.md)
4. [Markov chain](markov-chain-split.md)
5. [Markov process](markov-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Five-state harmonic absorption example](five-state-harmonic-absorption-example.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2/10f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-2/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/27k/ii/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/6/b/solution.md)
- [Solution](past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2021/section-b/6/c/solution.md)
- [Simple random walk on the integer line](simple-random-walk-on-the-integer-line.md)
