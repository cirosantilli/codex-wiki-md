<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A time-homogeneous [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) on a countable state space is a stochastic process with the [Markov property](../../../../../../markov-property.md): conditional on the current state, the law of its future depends on neither its past nor the current time. In the usual conservative, nonexplosive setting its sample paths are right-continuous step [functions](../../../../../../function-split.md). Its [Q-matrix](../../../../../../transition-rate-matrix.md) $Q=(q_{ij})$ has $q_{ij}\ge0$ for $j\ne i$, $q_i=-q_{ii}=\sum_{j\ne i}q_{ij}<\infty$, and infinitesimal transition probabilities $\mathbb P_i(X(h)=j)=q_{ij}h+o(h)$ for $j\ne i$.

On entering $i$, the [holding time](../../../../../../holding-time.md) has distribution $\operatorname{Exp}(q_i)$; independently, the next state is $j$ with [probability](../../../../../../probability.md) $q_{ij}/q_i$. The successive states form the [jump chain](../../../../../../jump-chain.md), whose transition probabilities are

$$
\boxed{p_{ij}=q_{ij}/q_i\quad(j\ne i),\qquad p_{ii}=0\quad(q_i>0)}.
$$

If $q_i=0$, the state is absorbing, its [holding time](../../../../../../holding-time.md) is infinite, and the jump-chain convention is $p_{ii}=1$. Nonexplosion ensures this construction defines the process for all finite times rather than accumulating infinitely many jumps in finite time.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
