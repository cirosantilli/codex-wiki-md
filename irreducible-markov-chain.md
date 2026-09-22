# Irreducible Markov chain

↑ **Parent:** [Markov chain](markov-chain-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Irreducible_Markov_chain)

For a finite, time-homogeneous [Discrete-time Markov chain](discrete-time-markov-chain.md) with row-stochastic [transition matrix](stochastic-matrix.md) $P$, irreducibility means

$$
\forall i,j\in S\quad\exists n\geq0:\quad(P^n)_{ij}>0.
$$

Equivalently, all states form one [communicating class](communicating-class.md). The step count may depend on $i,j$; irreducibility does not require every one-step [transition probability](transition-probability.md) to be positive. Drawing an arrow $i\to j$ whenever $P_{ij}>0$ makes the condition exactly that of a [strongly connected directed graph](strong-connectivity.md). It is a property of the entire chosen [state space](state-space.md), independent of the initial [probability distribution](probability-distribution-split.md).

Irreducibility describes where the [Markov chain](markov-chain-split.md) can travel; [aperiodicity](aperiodic-markov-chain.md) describes the possible lengths of return paths. For example, restricting the second diagram in [communicating class](communicating-class.md) to its closed pair $\{c_1,c_2\}$ gives

$$
C=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
C^{2k}=I,\qquad C^{2k+1}=C\quad(k\geq0),
$$

where $I$ is the [identity matrix](identity-matrix.md). This [Markov chain](markov-chain-split.md) is irreducible, but each state's [period of a state in a Markov chain](period-of-a-state-in-a-markov-chain.md) is two. Every destination is reachable, yet a given destination cannot be reached at every sufficiently large step count. Starting at $c_1$ produces alternating one-time [probability distributions](probability-distribution-split.md). See [Hao Wu's MIT lecture 2, irreducibility and periods](https://ocw.mit.edu/courses/18-445-introduction-to-stochastic-processes-spring-2015/2edaa8542469ce692226813a8bd1ec88_MIT18_445S15_lecture2.pdf) for the definitions.

Adding a [holding probability of a Markov chain](holding-probability-of-a-markov-chain.md) $\varepsilon$ at each state, with $0<\varepsilon<1$, gives

$$
C_\varepsilon=\varepsilon I+(1-\varepsilon)C.
$$

The arrows between the two states remain, so the [Markov chain](markov-chain-split.md) remains irreducible. A positive one-step return makes it an [aperiodic Markov chain](aperiodic-markov-chain.md). At $\varepsilon=1/2$, both rows are $(1/2,1/2)$ and $C_{1/2}^n=C_{1/2}$ for every $n\geq1$: the initial state is forgotten after one step. At $\varepsilon=1$, however, both states become [absorbing states](absorbing-state.md), giving two separate [communicating classes](communicating-class.md) and losing irreducibility.

For a [finite Markov chain](finite-markov-chain.md), irreducibility guarantees a unique [stationary distribution](stationary-distribution.md) with positive weight at every state. Adding [aperiodicity](aperiodic-markov-chain.md) guarantees convergence $\mu_0P^n\to\pi$ for every initial [probability distribution](probability-distribution-split.md); see [Hao Wu's MIT lecture 4, convergence theorem](https://ocw.mit.edu/courses/18-445-introduction-to-stochastic-processes-spring-2015/5bd4774f613aa28bd111c36f3a3beeed_MIT18_445S15_lecture4.pdf). The [Markov chain ergodic theorem](markov-chain-ergodic-theorem.md) gives convergence of empirical visit frequencies even for an irreducible periodic [Markov chain](markov-chain-split.md). These results explain why checking connectivity is a useful first step before studying equilibrium. Conversely, any [absorbing state](absorbing-state.md) prevents irreducibility if there is another state: it cannot reach that state. The one-state [Markov chain](markov-chain-split.md) is the exception.

**Table of contents**

- [Phi-irreducibility](phi-irreducibility.md)

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (58)

- [Absolute relaxation time](absolute-relaxation-time.md)
- [Bounded conditional moments imply a geometric drift](bounded-conditional-moments-imply-a-geometric-drift.md)
- [Communicating class](communicating-class.md)
- [Cooling schedule for simulated annealing](cooling-schedule-for-simulated-annealing.md)
- [Countable-state Markov chain convergence theorem](countable-state-markov-chain-convergence-theorem.md)
- [Eigenvalue lower bound for total variation mixing](eigenvalue-lower-bound-for-total-variation-mixing.md)
- [Ergodic theorem for a finite continuous-time Markov chain](ergodic-theorem-for-a-finite-continuous-time-markov-chain.md)
- [Fixed-temperature law of simulated annealing](fixed-temperature-law-of-simulated-annealing.md)
- [Fluid scaling proof of multiple Erlang fixed points](fluid-scaling-proof-of-multiple-erlang-fixed-points.md)
- [Gibbs sampling for a finite hidden spin field](gibbs-sampling-for-a-finite-hidden-spin-field.md)
- [Irreducibility and recurrence pass between a CTMC and its jump chain](irreducibility-and-recurrence-pass-between-a-ctmc-and-its-jump-chain.md)
- [Markov chain invariant measure](markov-chain-invariant-measure.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-34/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1/11h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1/11h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/11h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/22h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-2/20d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-2/20c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-45/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/27j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/27j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-28/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37/6/i/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/9h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/20h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/9h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-215/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-1/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/28k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/27k/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-219/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/27k/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/18h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-215/1/a/solution.md)
- [Peres product condition](peres-product-condition.md)
- [Poincare inequality for a reversible Markov chain](poincare-inequality-for-a-reversible-markov-chain.md)
- [Positive recurrent Markov chain](positive-recurrent-markov-chain.md)
- [Spectral kernel expansion of a reversible chain](spectral-kernel-expansion-of-a-reversible-chain.md)
- [Stationary distribution](stationary-distribution.md)
