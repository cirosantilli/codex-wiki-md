<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Let $X_n=S_n\bmod4$. The residue contains all information needed for the next residue, so $(X_n)$ is a four-state [Markov chain](../../../../../markov-chain.md). In the order $0,1,2,3$, its [transition matrix](../../../../../stochastic-matrix.md) is

$$
P=\begin{pmatrix}
1/2&1/2&0&0\\
0&1/2&1/2&0\\
1/2&0&0&1/2\\
1/2&0&0&1/2
\end{pmatrix}.
$$

For example, from residue $2$, a head returns to $0$ and a tail goes to $3$; from either odd residue the tail leaves that residue unchanged.

The [stationary distribution](../../../../../stationary-distribution.md) $\pi$ solves $\pi P=\pi$. Its equations give $\pi_1=\pi_0$, $\pi_2=\pi_1/2$, and $\pi_3=\pi_2$. Normalization therefore gives

$$
\boxed{\pi=(1/3,1/3,1/6,1/6).}
$$

The [Markov chain](../../../../../markov-chain.md) is irreducible: the positive-probability transitions around $0\to1\to2\to3\to0$ reach all states. It is also aperiodic because it has self-loops. The finite irreducible [Markov chain ergodic theorem](../../../../../markov-chain-ergodic-theorem.md) says that empirical state frequencies converge almost surely to the unique [stationary distribution](../../../../../stationary-distribution.md), irrespective of the initial state. Hence

$$
\boxed{\lim_{N\to\infty}\frac1N\sum_{n=1}^N\mathbf1_{\{4\mid S_n\}}=\frac13\quad\text{almost surely}.}
$$

Aperiodicity also permits convergence of the one-time state probabilities, although it is not needed for this empirical-frequency theorem.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
