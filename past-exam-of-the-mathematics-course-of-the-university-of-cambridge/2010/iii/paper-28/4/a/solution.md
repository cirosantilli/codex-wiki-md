<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $T_\pi$ permute coordinates $0,\ldots,m$, fixing the later coordinates. For any integrable [random variable](../../../../../../random-variable-split.md) $V$, its group average

$$
A_mV=\frac1{(m+1)!}\sum_{\pi\in S_{m+1}}V\circ T_\pi
$$

is invariant under this group, hence $\mathcal S_m$-measurable. If $C\in\mathcal S_m$, invariance of $C$ and measure preservation of each $T_\pi$ give $\mathbb E[\mathbf1_CV\circ T_\pi]=\mathbb E[\mathbf1_CV]$. Thus $A_mV$ satisfies the integral definition of $\mathbb E[V\mid\mathcal S_m]$. This proves [symmetrization as conditional expectation](../../../../../../symmetrization-as-conditional-expectation.md).

Apply it to $V=\mathbf1_{A_k}(X_k)$ for $m\geq k$. Under a uniform [permutation](../../../../../../permutation.md) of $m+1$ coordinates, its selected coordinate is uniform among all of them, so

$$
\mathbb E[\mathbf1_{A_k}(X_k)\mid\mathcal S_m]
=\frac1{m+1}\sum_{j=0}^m\mathbf1_{A_k}(X_j)
=\frac{S_m^k}{m+1}.
$$

The [reverse martingale convergence theorem](../../../../../../reverse-martingale-convergence-theorem.md) says that, for decreasing sigma-algebras $\mathcal H_m$ and an integrable $V$, these conditional expectations converge [almost surely](../../../../../../almost-sure-convergence.md) and in $L^1$ to $\mathbb E[V\mid\bigcap_m\mathcal H_m]$. Here $\mathcal S_m\downarrow\mathcal S$, because every finitely supported permutation belongs to one of the finite groups. Therefore

$$
\boxed{\frac{S_m^k}{m+1}\longrightarrow\mathbb E[\mathbf1_{A_k}(X_k)\mid\mathcal S]\quad\text{almost surely and in }L^1.}
$$

Intersect these probability-one events for the finitely many $k=0,\ldots,p$ and multiply the limits. Expanding the product of finite sums gives

$$
\boxed{\prod_{k=0}^p\mathbb E[\mathbf1_{A_k}(X_k)\mid\mathcal S]
=\lim_{m\to\infty}\frac1{(m+1)^{p+1}}
\sum_{0\leq\ell_0,\ldots,\ell_p\leq m}\prod_{k=0}^p\mathbf1_{A_k}(X_{\ell_k})\quad\text{almost surely}.}
$$

The sum here includes repeated indices. No independence of the original coordinates was assumed; exchangeability and reverse conditional-expectation convergence are precisely what replaced it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
