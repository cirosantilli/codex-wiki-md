<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

For a [Markov chain invariant measure](../../../../../markov-chain-invariant-measure.md), $xP=x$, and hence $xP^n=x$. The [irreducible Markov chain](../../../../../irreducible-markov-chain.md) property supplies, for each $j$, an $n$ with $(P^n)_{kj}>0$. Nonnegativity gives $x_j\ge x_k(P^n)_{kj}>0$. **Every coordinate of a nonzero invariant measure is positive.**

Start the [Markov chain](../../../../../markov-chain.md) at $k$, and let $T_k=\inf\{n\ge1:X_n=k\}$ be its first return time. Each product in the series is the probability of a path with no intermediate visit to $k$. Thus

$$
\gamma_j^k=\sum_{n\ge1}\mathbb P_k(X_n=j,\ T_k\ge n)
=\mathbb E_k\left[\sum_{n=1}^{T_k}\mathbf1_{\{X_n=j\}}\right].
$$

This is the expected number of visits to $j$ in an excursion, including the return endpoint and excluding the starting point. Because the chain is [recurrent Markov chain](../../../../../recurrent-markov-chain.md), $T_k<\infty$ almost surely, and exactly one visit to $k$ is counted: **$\gamma_k^k=1$**. Counting the starting point instead of the return endpoint gives the equivalent usual [excursion occupation measure](../../../../../excursion-occupation-measure.md).

For the lower bound, let $J=I\setminus\{k\}$, $Q=(p_{ij})_{i,j\in J}$, and $r=(p_{kj})_{j\in J}$. The stationarity equations on $J$, with $x_k=1$, are $x_J=r+x_JQ$. Iterating and using nonnegativity yields

$$
x_J=r+rQ+\cdots+rQ^{N-1}+x_JQ^N\ \ge\ \sum_{m=0}^{N-1}rQ^m.
$$

The $j$th coordinate on the right is precisely the partial excursion series for $j\ne k$. Taking its increasing limit gives **$x_j\ge\gamma_j^k$**; for $j=k$ equality follows from $x_k=\gamma_k^k=1$. The iteration is valid also on a countable state space because all summands are nonnegative.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
