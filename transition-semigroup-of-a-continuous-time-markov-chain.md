# Transition semigroup of a continuous-time Markov chain

↑ **Parent:** [Continuous-time Markov chain](continuous-time-markov-chain.md)

For a time-homogeneous [continuous-time Markov chain](continuous-time-markov-chain.md), $P_{ij}(t)=\mathbb P_i(X_t=j)$ and the [matrices](matrix.md) satisfy $P(s+t)=P(s)P(t)$, the [Chapman-Kolmogorov equation](chapman-kolmogorov-equation.md). On a finite [state space](state-space.md) with [Q-matrix](transition-rate-matrix.md) $Q$, the [matrix exponential](matrix-exponential.md) gives $P(t)=e^{tQ}$.

The distinction from a discrete-time [transition matrix](stochastic-matrix.md) is the elapsed-time parameter: $P(t)$ describes where the process is after $t$ time units, allowing any number of intervening jumps. Each $P(t)$ is a [stochastic matrix](stochastic-matrix.md), with $P(0)=I$. A [Q-matrix](transition-rate-matrix.md) instead records instantaneous rates and has row sums zero. Sampling at a fixed spacing $\Delta$ yields a [Discrete-time Markov chain](discrete-time-markov-chain.md) with [transition matrix](stochastic-matrix.md) $P(\Delta)$. See [Hao Wu's MIT lecture 21, transition semigroups](https://ocw.mit.edu/courses/18-445-introduction-to-stochastic-processes-spring-2015/245cbb8888672b1b902c308fd6e2468f_MIT18_445S15_lecture21.pdf) and [lecture 22, infinitesimal rates](https://ocw.mit.edu/courses/18-445-introduction-to-stochastic-processes-spring-2015/f6b1c125c2b471928e960a1d2c8ea6b5_MIT18_445S15_lecture22.pdf).

**Table of contents**

- [Poisson-sampled continuous-time Markov chain](poisson-sampled-continuous-time-markov-chain.md)
- [Kolmogorov equations](kolmogorov-equations.md)

## ↑ Ancestors (8)

1. [Continuous-time Markov chain](continuous-time-markov-chain.md)
2. [Markov chain](markov-chain.md)
3. [Markov process](markov-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Markov semigroup](markov-semigroup.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/27j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/28j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-207/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207/1/f/i/solution.md)
