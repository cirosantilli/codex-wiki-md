<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<i<N$, the total rate out of $i$ is $\lambda_i$. The [holding time](../../../../../../holding-time.md) of the [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) and its next state satisfy

$$
\boxed{J_i\sim\operatorname{Exp}(\lambda_i),\qquad
\mathbb P_i(X_{J_i}=i-1)=\mathbb P_i(X_{J_i}=i+1)=\frac12.}
$$

The [holding time](../../../../../../holding-time.md) is [independent](../../../../../../independent-random-variables.md) of the direction of this jump: the conditional probability of destination $j$ is the rate $q_{ij}$ divided by the total rate $\lambda_i$, independently of the elapsed holding duration. This is the exponential-clock construction of a [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) with the given [infinitesimal generator matrix](../../../../../../transition-intensity-matrix.md).

At $i=0$ or $i=N$, all rates out are zero. These are [absorbing states](../../../../../../absorbing-state.md); the path remains at its initial endpoint and $J_i=\infty$ [almost surely](../../../../../../almost-sure-convergence.md). There is no next visited state, so $X_{J_i}$ is not a finite-time jump value at either endpoint. If one separately uses $X_\infty$ for the limiting state, that limit is the same endpoint.

The embedded jump chain in the interior is a [simple symmetric random walk](../../../../../../simple-symmetric-random-walk.md) on $\{0,\ldots,N\}$, stopped at the endpoints. From any interior state it has probability at least $2^{-N}$ of hitting a boundary in the next $N$ jumps, by following successive leftward choices. Thus its number of jumps before absorption is finite [almost surely](../../../../../../almost-sure-convergence.md). Each of this finite number of [holding times](../../../../../../holding-time.md) is finite [almost surely](../../../../../../almost-sure-convergence.md), so absorption also occurs in finite continuous time. The finite set of positive interior rates causes no explosion; in particular their maximum bounds the total jump rate. When $N=1$, the chain starts at an already absorbing endpoint.

The rates alter the clock but not the sequence of visited states. The [gambler's ruin](../../../../../../gambler-s-ruin.md) calculation from part (a), translated to an initial state $i$ between endpoints $0,N$, therefore gives

$$
\boxed{\mathbb P_i(E)=\frac{N-i}{N}\qquad(0\leq i\leq N).}
$$

This includes probability one at zero and probability zero at $N$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
