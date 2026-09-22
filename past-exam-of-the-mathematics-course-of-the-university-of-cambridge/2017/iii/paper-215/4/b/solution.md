<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [symmetric group](../../../../../../symmetric-group.md) has $n!$ elements, not the printed order $n$. For $n\geq2$ the identity and the $n-1$ adjacent [transpositions](../../../../../../transposition-permutation.md) have probabilities $1/n$, so the specified [transition matrix](../../../../../../stochastic-matrix.md) is normalized. Its [stationary distribution](../../../../../../stationary-distribution.md) is uniform and it satisfies [detailed balance](../../../../../../detailed-balance.md), since each [transposition](../../../../../../transposition-permutation.md) is its own inverse. Adjacent [transpositions](../../../../../../transposition-permutation.md) generate the [symmetric group](../../../../../../symmetric-group.md), making this an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md); the positive holding probability makes it an [aperiodic Markov chain](../../../../../../aperiodic-markov-chain.md).

For a fixed label $i$, right multiplication swaps positions, so $f(\sigma)=\sigma^{-1}(i)$ is the label's position. Under the [uniform distribution on a finite set](../../../../../../discrete-uniform-distribution.md) it is uniform on $\{1,\ldots,n\}$. Therefore

$$
\pi(f)=\frac{n+1}{2},\qquad\operatorname{Var}_\pi(f)=\frac{n^2-1}{12}.
$$

For each generator $s_j=(j,j+1)$, the squared change $[f(\sigma s_j)-f(\sigma)]^2$ is one if the label occupies either of the two positions, and zero otherwise. Its stationary [expected value](../../../../../../expected-value.md) is $2/n$, giving

$$
\mathcal E(f,f)=\frac12\sum_{j=1}^{n-1}\frac1n\frac2n=\frac{n-1}{n^2}.
$$

Thus the [tagged-label Rayleigh quotient for adjacent transpositions](../../../../../../tagged-label-rayleigh-quotient-for-adjacent-transpositions.md) gives the corrected bound

$$
\boxed{\gamma\leq\frac{12}{n^2(n+1)}=\frac{12}{n^3}(1+o(1)).}
$$

The printed factor six cannot be obtained: the hint's [variance of a uniform distribution](../../../../../../variance-of-a-uniform-distribution.md) is wrong. Directly, $\operatorname{Var}(U)=\int_0^1u^2\,du-(\int_0^1u\,du)^2=1/12$. Bounded [convergence in distribution](../../../../../../convergence-in-distribution.md) of $U_n$ does imply convergence of its first two moments, hence convergence of its [variance](../../../../../../variance-split.md), but the limit is $1/12$.

More strongly, the claimed asymptotic bound itself is false for this kernel. The [Aldous spectral gap theorem](../../../../../../aldous-spectral-gap-theorem.md) states that the [interchange process](../../../../../../interchange-process.md) on a finite connected weighted [graph](../../../../../../graph-split.md) has the same [spectral gap](../../../../../../spectral-gap.md) as the single-label [random walk](../../../../../../random-walk.md) with identical edge rates; see [Theorem 1.1 and its proof](https://arxiv.org/abs/0906.1238). Here $P-I$ is that [interchange process](../../../../../../interchange-process.md) generator on a [path graph](../../../../../../path-graph.md) with edge rates $1/n$. For the tagged-label generator, direct substitution of $g_\ell(k)=\cos(\ell\pi(k-1/2)/n)$ gives [eigenvalues](../../../../../../eigenvalue.md) $-2(1-\cos(\ell\pi/n))/n$, $0\leq\ell<n$, including the reflecting endpoint equations. These $n$ distinct [eigenvalues](../../../../../../eigenvalue.md) exhaust the tagged-label function space. Consequently the theorem yields

$$
\boxed{\gamma=\frac2n\left(1-\cos\frac\pi n\right)\sim\frac{\pi^2}{n^3},}
$$

which exceeds $6/n^3$ asymptotically. This use of a substantial external theorem is only to certify the printed claim's failure; the corrected factor-twelve upper bound above follows directly from the requested test function and the variational formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
