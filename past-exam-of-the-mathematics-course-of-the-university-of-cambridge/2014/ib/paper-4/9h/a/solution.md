<h1 id="9h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Markov property](../../../../../../markov-property.md) and the [Chapman-Kolmogorov equation](../../../../../../chapman-kolmogorov-equation.md) give

$$
 \mathbb P(X_{2n+2}=j\mid X_{2n}=i,X_{2n-2},\ldots,X_0)
 =\sum_{k\in S}p_{ik}p_{kj}=(P^2)_{ij}.
$$

For each intermediate state, one first uses the next-step [transition probability](../../../../../../transition-probability.md) and then the following one; the sampled history adds no information once $X_{2n}$ is known. Thus $W$ is a homogeneous [Markov chain](../../../../../../markov-chain.md) with [transition matrix](../../../../../../stochastic-matrix.md) $P^2$ and initial law $\lambda$. In particular,

$$
 \boxed{\mathbb P(W_1=0)=\sum_{i\in S}\lambda_i\sum_{j\in S}p_{ij}p_{j0}.}
$$

If zero is not a state of $S$, this probability is zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9H](../../9h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
