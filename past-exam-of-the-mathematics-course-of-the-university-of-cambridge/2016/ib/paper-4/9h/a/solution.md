<h1 id="9h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If there are $i$ balls in box A, a ball currently in B is selected with probability $(k-i)/k$, increasing the count, and a ball in A is selected with probability $i/k$, decreasing it. For $k\geq1$,

$$
\boxed{P_{i,i+1}=\frac{k-i}{k}\ (0\leq i<k),\qquad P_{i,i-1}=\frac{i}{k}\ (0<i\leq k),}
$$

with every other transition zero. This is the [Ehrenfest urn model](../../../../../../ehrenfest-urn-model.md).

The [stationary distribution](../../../../../../stationary-distribution.md) is

$$
\boxed{\pi_i=2^{-k}\binom ki,\qquad 0\leq i\leq k.}
$$

It is normalized by the [binomial theorem](../../../../../../binomial-theorem.md), and it obeys the [detailed balance](../../../../../../detailed-balance.md):

$$
\pi_iP_{i,i+1}=2^{-k}\binom ki\frac{k-i}{k}=2^{-k}\binom k{i+1}\frac{i+1}{k}=\pi_{i+1}P_{i+1,i}.
$$

All other pairs have zero flux in both directions. These identities prove stationarity and show that this is a [reversible Markov chain](../../../../../../reversible-markov-chain.md) in equilibrium. The finite chain is irreducible and has period two; reversibility does not require aperiodicity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9H](../../9h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
