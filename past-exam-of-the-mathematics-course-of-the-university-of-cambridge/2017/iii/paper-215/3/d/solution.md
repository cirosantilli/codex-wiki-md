<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each [subset](../../../../../../subset.md) $J\subseteq\{1,\ldots,n\}$, take the [Walsh character](../../../../../../walsh-character.md) $f_J(x)=\prod_{j\in J}x_j$, including $f_\varnothing\equiv1$. Under the [uniform distribution on a finite set](../../../../../../discrete-uniform-distribution.md) these functions are an [orthonormal basis](../../../../../../orthonormal-basis.md): $f_Jf_K=f_{J\triangle K}$ has mean zero unless $J=K$, since the coordinates are independent fair signs. There are $2^n$ such functions, the full dimension of the function space.

Flipping a coordinate in $J$ changes the sign, while flipping one outside $J$ leaves the value unchanged. The total probability of a sign change is $|J|/(2n)$, so

$$
Pf_J=\left(1-\frac{|J|}{n}\right)f_J.
$$

The [spectrum of lazy random walk on the hypercube](../../../../../../spectrum-of-lazy-random-walk-on-the-hypercube.md) is therefore

$$
\boxed{\lambda_k=1-\frac{k}{n}\quad\text{with multiplicity }\binom nk,\quad0\leq k\leq n.}
$$

All [eigenvalues](../../../../../../eigenvalue.md) are nonnegative and the second largest is $1-1/n$. Hence both the ordinary [spectral gap](../../../../../../spectral-gap.md) and the absolute [spectral gap](../../../../../../spectral-gap.md) equal $\boxed{\gamma=1/n}$. The requested bound in part (c) is smaller than the exact gap by a factor $2n$; even the refined increasing-coordinate [canonical paths Poincare bound](../../../../../../canonical-paths-poincare-bound.md) loses a factor $(n+1)/2$. The true optimal [Poincare inequality for a reversible Markov chain](../../../../../../poincare-inequality-for-a-reversible-markov-chain.md) constant is $n$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
