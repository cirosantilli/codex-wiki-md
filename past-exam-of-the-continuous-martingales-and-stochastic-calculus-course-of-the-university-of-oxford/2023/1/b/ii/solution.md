<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Enumerate the [orthonormal basis](../../../../../orthonormal-basis.md) consisting of $H_0$ and the [Haar wavelets](../../../../../haar-wavelet.md) $H_{n,k}$ as $(e_j)_{j\geq1}$, and enumerate the corresponding [independent](../../../../../independent-random-variables.md) [standard normal random variables](../../../../../standard-normal-random-variable.md) as $(A_j)_{j\geq1}$. Set $c_j=\langle h,e_j\rangle_{\mathcal H}$. The [Parseval identity for a Hilbertian basis](../../../../../parseval-identity-for-a-hilbertian-basis.md) gives

$$
\sum_{j=1}^\infty c_j^2=\|h\|_{\mathcal H}^2<\infty.
$$

The partial sums $T_m=\sum_{j=1}^mc_jA_j$ form a [martingale](../../../../../martingale-split.md) for $\sigma(A_1,\ldots,A_m)$, since the next summand is [independent](../../../../../independent-random-variables.md) of the past and has [mean](../../../../../expected-value-split.md) zero. Moreover,

$$
\mathbb ET_m^2=\sum_{j=1}^mc_j^2\leq\|h\|_{\mathcal H}^2.
$$

The [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) for a [martingale](../../../../../martingale-split.md) bounded in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) proves convergence [almost surely](../../../../../almost-sure-convergence.md) and [convergence in L2](../../../../../convergence-in-l2.md). Equivalently one may apply the [Kolmogorov convergence theorem](../../../../../kolmogorov-convergence-theorem.md) to the summable [variances](../../../../../variance-split.md) $c_j^2$.

A finite [linear combination of independent normal random variables](../../../../../linear-combination-of-independent-normal-random-variables.md) is normal. Its [characteristic function](../../../../../characteristic-function-split.md) is $\mathbb E e^{iuT_m}=\exp(-u^2\sum_{j\leq m}c_j^2/2)$. Passing to the limit identifies

$$
\boxed{Wh=\lim_{m\to\infty}T_m\quad\text{almost surely and in }L^2(\mathbb P),
\qquad Wh\sim N(0,\|h\|_{\mathcal H}^2).}
$$

For $h=0$ this is the constant zero [random variable](../../../../../random-variable-split.md). Each fixed $h$ has its own permissible null set; simultaneous pathwise convergence for all $h\in\mathcal H$ is unnecessary.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
