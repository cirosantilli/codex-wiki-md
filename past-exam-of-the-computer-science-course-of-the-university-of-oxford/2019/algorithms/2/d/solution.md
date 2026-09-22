<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $B=A^T$ and choose any column [probability vector](../../../../../probability-vector.md) $q$, for example the first coordinate [unit vector](../../../../../unit-vector.md). Because $A$ has nonnegative entries and each row sums to one, $B$ maps the [probability simplex](../../../../../probability-simplex.md)

$$
\Delta=\{v\in\mathbb R^n:v\geq0,\ \mathbf1^Tv=1\}
$$

into itself: $Bv\geq0$ and $\mathbf1^TBv=(A\mathbf1)^Tv=\mathbf1^Tv=1$.

The iterates $B^jq$ need not converge, so take their arithmetic averages,

$$
x_N=\frac1N\sum_{j=0}^{N-1}B^jq\in\Delta.
$$

A telescoping [sum](../../../../../sum.md) gives

$$
Bx_N-x_N=\frac{B^Nq-q}{N}.
$$

Both [vectors](../../../../../vector.md) on the right before subtraction have [L1 norm](../../../../../l1-norm.md) one, so $\|Bx_N-x_N\|_1\leq2/N\to0$.

The [probability simplex](../../../../../probability-simplex.md) is closed and bounded in finite-dimensional [Euclidean space](../../../../../euclidean-norm.md), hence compact by the [Heine-Borel theorem](../../../../../heine-borel-theorem.md). It follows that a [subsequence](../../../../../subsequence.md) $x_{N_j}$ converges to some $x\in\Delta$. Passing to the [limit](../../../../../limit-of-a-function.md) in the displayed identity, using [continuity](../../../../../continuous-function.md) of the [linear map](../../../../../linear-map.md) $B$, gives **$A^Tx=Bx=x$, with $x\geq0$ and $\sum_i x_i=1$**.

This proves [stationary distribution existence for a finite Markov chain](../../../../../stationary-distribution-existence-for-a-finite-markov-chain.md) without any [Markov chain irreducibility](../../../../../irreducible-markov-chain.md) or [aperiodicity](../../../../../aperiodic-markov-chain.md) assumption. Those stronger hypotheses concern uniqueness and convergence, not the existence required here.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
