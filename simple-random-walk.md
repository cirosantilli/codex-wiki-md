# Simple random walk

↑ **Parent:** [Random walk on a graph](random-walk-on-a-graph.md)

A simple random walk on a [locally finite graph](locally-finite-graph.md) chooses each [vertex](vertex-graph-theory.md) in the current [vertex](vertex-graph-theory.md)'s [graph neighbourhood](graph-neighbourhood.md) with equal [probability](probability.md), assuming there is at least one available [neighbour](neighbour-of-a-vertex.md). On the [integer](integer.md) line there are two choices, one unit left or right, so each has [probability](probability.md) $1/2$. This is the one-dimensional [simple symmetric random walk](simple-symmetric-random-walk.md). Terminology varies: a [simple random walk on the integer line](simple-random-walk-on-the-integer-line.md) is also often allowed unequal step [probabilities](probability.md), with “symmetric” specifying the fair case.

For a [simple symmetric random walk](simple-symmetric-random-walk.md) starting at $S_0=0$, each [increment](increment.md) has the [Rademacher distribution](rademacher-distribution.md), with [expected value](expected-value.md) zero and [variance](variance-split.md) one. Thus [linearity of expectation](linearity-of-expectation.md) and the [variance of a sum](variance-of-a-sum.md) of [independent random variables](independent-random-variables.md) give

$$
\mathbb E S_n=0,\qquad \operatorname{Var}(S_n)=n,\qquad \sigma_n=\sqrt n.
$$

For example, after $80$ steps the [expected value](expected-value.md) is zero, the [variance](variance-split.md) is $80$, and the [standard deviation](standard-deviation.md) is $\sqrt{80}\approx8.944$. Doubling the typical distance scale takes four times as many steps. This square-root growth explains why a [random walk](random-walk.md) can wander far even when there is no preferred direction.

<a id="image-four-fair-and-two-biased-unit-step-random-walk-paths-with-their-expected-values-and-bands-one-standard-deviation-wide-on-either-side"></a>
![](random-walk-paths-and-drift.png)

**[Figure 5](#image-four-fair-and-two-biased-unit-step-random-walk-paths-with-their-expected-values-and-bands-one-standard-deviation-wide-on-either-side). Four fair and two biased unit-step random-walk paths, with their expected values and bands one standard deviation wide on either side.**

The colored curves are illustrative [sample paths](sample-path.md), not averages over all possible walks. The dashed curves show the [expected values](expected-value.md); the shaded bands show the [expected value](expected-value.md) plus or minus one [standard deviation](standard-deviation.md) at each time. These bands are a scale of spread, not [confidence intervals](confidence-interval.md), and give no guarantee that an entire [sample path](sample-path.md) stays inside them.

Zero [expected value](expected-value.md) does not make this a [stationary process](stationary-process.md): its one-time [probability distribution](probability-distribution.md) changes with $n$, as the increasing [variance](variance-split.md) already proves. It does have [stationary increments](stationary-increments.md) and [independent increments](independent-increments.md), because blocks of fresh steps have the same [probability distribution](probability-distribution.md) at any starting time and disjoint blocks use [independent random variables](independent-random-variables.md). This separation of position from [increment](increment.md) is one reason the [random walk](random-walk.md) is such a useful first example of a [stochastic process](stochastic-process-split.md).

**Table of contents**

- [Simple symmetric random walk](simple-symmetric-random-walk.md)
  - [Multinomial collision proof of three-dimensional walk transience](multinomial-collision-proof-of-three-dimensional-walk-transience.md)
  - [Infinite mean first passage of a simple symmetric random walk](infinite-mean-first-passage-of-a-simple-symmetric-random-walk.md)
  - [Origin capture by a sufficiently sleepy planar random walk](origin-capture-by-a-sufficiently-sleepy-planar-random-walk.md)
  - [Exponential maximal bound for a symmetric random walk](exponential-maximal-bound-for-a-symmetric-random-walk.md)
  - [First-return generating function of the simple symmetric random walk](first-return-generating-function-of-the-simple-symmetric-random-walk.md)
  - [Expected time to expand a random-walk range](expected-time-to-expand-a-random-walk-range.md)
  - [Square-minus-time martingale of a simple symmetric random walk](square-minus-time-martingale-of-a-simple-symmetric-random-walk.md)
    - [Stopped second-moment identity for a simple symmetric random walk](stopped-second-moment-identity-for-a-simple-symmetric-random-walk.md)
- [Simple random walk on the hypercube](simple-random-walk-on-the-hypercube.md)
  - [Spectrum of lazy random walk on the hypercube](spectrum-of-lazy-random-walk-on-the-hypercube.md)
- [Simple random walk in two dimensions is recurrent](simple-random-walk-in-two-dimensions-is-recurrent.md)

## ↑ Ancestors (9)

1. [Random walk on a graph](random-walk-on-a-graph.md)
2. [Random walk](random-walk.md)
3. [Markov chain](markov-chain.md)
4. [Markov process](markov-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (29)

- [Biased random walk](biased-random-walk.md)
- [Brownian scaling](brownian-scaling.md)
- [Directed edge occupation in a random-walk commute](directed-edge-occupation-in-a-random-walk-commute.md)
- [Expected cover time of a cycle](expected-cover-time-of-a-cycle.md)
- [Graph exhaustion](graph-exhaustion.md)
- [Green-function decay for simple random walk on the integer lattice](green-function-decay-for-simple-random-walk-on-the-integer-lattice.md)
- [Hitting time of the bridge vertex between two cliques](hitting-time-of-the-bridge-vertex-between-two-cliques.md)
- [Killed-walk occupation voltage](killed-walk-occupation-voltage.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/29i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/9h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-214/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-2/12f/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-214/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-2/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/9h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/19h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-209/4/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-212/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-226/1/a/solution.md)
- [Ratio definition of cutoff](ratio-definition-of-cutoff.md)
- [Recurrent graph](recurrent-graph.md)
- [Transient graph](transient-graph.md)
