# Discrete-time Markov chain

↑ **Parent:** [Markov chain](markov-chain-split.md)

A time-homogeneous [Discrete-time Markov chain](discrete-time-markov-chain.md) is a sequence of [random variables](random-variable-split.md) $Y_0,Y_1,\ldots$ indexed by nonnegative [integers](integer-split.md), with the displayed [conditional probabilities](conditional-probability.md). Here $\mathcal F_n$ is its [natural filtration](natural-filtration.md) and $P$ is a row-stochastic [transition matrix](stochastic-matrix.md). The [Markov property](markov-property.md) removes dependence on earlier observations once $Y_n$ is specified; the [time-homogeneous Markov property](time-homogeneous-markov-property.md) makes $P$ independent of $n$.

Consider states $S$ (sunny) and $R$ (rainy), with the constructed [transition matrix](stochastic-matrix.md)

$$
P=\begin{pmatrix}0.8&0.2\\0.4&0.6\end{pmatrix}.
$$

Rows give today's state and columns tomorrow's, in order $S,R$. These numbers define an illustrative model, with one step interpreted as one day; they are not estimates of real weather. Let $q_n=\mathbb P(Y_n=S)$. The [law of total probability](law-of-total-probability.md) gives the [recurrence relation](recurrence-relation.md)

$$
q_{n+1}=0.8q_n+0.4(1-q_n)=0.4+0.4q_n.
$$

Subtracting $2/3$ makes the deviation multiply by $0.4$ at each step. Thus

$$
q_n=\frac23+\left(q_0-\frac23\right)0.4^n.
$$

Starting sunny gives $q_0=1$, $q_1=0.8$, $q_2=0.72$ and $q_3=0.688$; starting rainy gives $q_0=0$ and $q_2=0.56$. The two predictions approach the same [stationary distribution](stationary-distribution.md) while retaining a shrinking trace of the initial [probability distribution](probability-distribution-split.md).

<a id="image-constructed-sunny-rainy-transitions-and-the-exact-sunny-probabilities-from-three-initial-distributions"></a>
![](markov-chain-convergence.png)

**[Figure 3](#image-constructed-sunny-rainy-transitions-and-the-exact-sunny-probabilities-from-three-initial-distributions). Constructed sunny/rainy transitions and the exact sunny probabilities from three initial distributions.**

An [expected hitting time](expected-hitting-time.md) answers a different question. Starting sunny, let $T_R=\inf\{n\geq0:Y_n=R\}$. Every day before the first rain remains sunny, so

$$
\mathbb P_S(T_R=k)=0.8^{k-1}0.2\quad(k\geq1).
$$

This [geometric distribution](geometric-distribution.md) has finite [expected value](expected-value-split.md). A first-step calculation gives $h_S=1+0.8h_S+0.2h_R$, with $h_R=0$, hence $h_S=5$ days. The same result follows from the [geometric series](geometric-series.md) $\mathbb E_ST_R=\sum_{n\geq0}0.8^n=5$. This is a mean waiting time, not a prediction that rain first occurs exactly five days later.

A [probability](probability.md) row [vector](vector.md) $\pi$ is a [stationary distribution](stationary-distribution.md) when $\pi P=\pi$. The [Markov chain](markov-chain-split.md) is [reversible](reversible-markov-chain.md) in that law when [detailed balance](detailed-balance.md) holds: $\pi_iP_{ij}=\pi_jP_{ji}$. Multiplying those equations along a finite path gives equal forward and reversed stationary path [probabilities](probability.md).

## ↑ Ancestors (7)

1. [Markov chain](markov-chain-split.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Absorbing state](absorbing-state.md)
- [Accessible state of a Markov chain](accessible-state-of-a-markov-chain.md)
- [Communicating class](communicating-class.md)
- [Discrete-time Markov chain](discrete-time-markov-chain.md)
- [Irreducible Markov chain](irreducible-markov-chain.md)
- [Markov chain](markov-chain-split.md)
- [No claims discount system](no-claims-discount-system.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-27/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-45/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/26i/iii/solution.md)
- [Stationary distribution](stationary-distribution.md)
- [Stochastic matrix](stochastic-matrix.md)
- [Transition semigroup of a continuous-time Markov chain](transition-semigroup-of-a-continuous-time-markov-chain.md)
