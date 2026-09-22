# Harmonic function for a Markov chain

↑ **Parent:** [Markov chain](markov-chain.md)

A harmonic function assigns a value to each state of a [Markov chain](markov-chain.md) such that one transition leaves its [expected value](expected-value.md) unchanged. This turns a question about many possible future [sample paths](sample-path.md), such as which endpoint is reached first, into a local averaging rule. For a [transition matrix](stochastic-matrix.md) $P$, a real-valued [function](function-split.md) $h$ is harmonic at state $i$ when

$$
h(i)=(Ph)(i)=\sum_jP_{ij}h(j)=\mathbb E_i[h(X_1)].
$$

Here $\mathbb E_i$ means [expected value](expected-value.md) conditional on starting at $X_0=i$; on a [countable](countable-set.md) [state space](state-space.md) the sum must be absolutely convergent. If this holds at every state, write $Ph=h$. At an [absorbing state](absorbing-state.md) the equation is automatic, so prescribed [boundary conditions](boundary-condition.md) supply information that the averaging rule cannot.

For a [finite Markov chain](finite-markov-chain.md), choose a boundary set $B$ that can be reached from every state, and assign boundary values $b$. If $T_B$ is its first [hitting time](first-passage-time.md), the harmonic extension is

$$
h(i)=\mathbb E_i[b(X_{T_B})],\qquad h|_B=b.
$$

Choosing $b$ to be the [indicator function](indicator-function.md) of one target within $B$ gives a [hitting probability](hitting-probability.md). This is a discrete [Dirichlet problem](dirichlet-problem.md): enforce the averaging rule outside $B$ and fix the values on $B$. See [Hao Wu's MIT lecture 8, harmonic extension, slide 5](https://ocw.mit.edu/courses/18-445-introduction-to-stochastic-processes-spring-2015/bc4e626fedc9aa9bb62c96e80fbd6ac0_MIT18_445S15_lecture8.pdf). The construction extends the mean-value idea of a [harmonic function](harmonic-function.md); for a [random walk on a graph](random-walk-on-a-graph.md) it is a [discrete harmonic function](discrete-harmonic-function.md).

**Table of contents**

- [Five-state harmonic absorption example](five-state-harmonic-absorption-example.md)

## ↑ Ancestors (7)

1. [Markov chain](markov-chain.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21/2/solution.md)
- [Period-two martingale corrector for a birth-death chain](period-two-martingale-corrector-for-a-birth-death-chain.md)
- [Scale increments for a birth-death chain](scale-increments-for-a-birth-death-chain.md)
