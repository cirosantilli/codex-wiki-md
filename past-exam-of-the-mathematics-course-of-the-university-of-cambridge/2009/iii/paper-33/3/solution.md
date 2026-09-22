<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\phi$ be the [scaling function](../../../../../scaling-function.md) and $\psi$ an [orthonormal wavelet](../../../../../orthonormal-wavelet.md), with $\phi_{j,k}(x)=2^{j/2}\phi(2^jx-k)$ and $\psi_{j,k}(x)=2^{j/2}\psi(2^jx-k)$. For $f\in L^2(\mathbb R)$, the [wavelet series](../../../../../wavelet-series.md) at a coarse level $j_0$ is

$$
f=\sum_{k\in\mathbb Z}\langle f,\phi_{j_0,k}\rangle\phi_{j_0,k}
+\sum_{j\ge j_0}\sum_{k\in\mathbb Z}\langle f,\psi_{j,k}\rangle\psi_{j,k}.
$$

The series converges in the [L2 norm](../../../../../l2-norm.md). Its coarse part captures broad variation and successive wavelet levels add finer detail. Truncating at levels $j<J$ produces the [orthogonal projection](../../../../../orthogonal-projection.md) onto $V_J$; [Parseval identity](../../../../../parseval-identity.md) makes its squared approximation error the sum of the omitted squared coefficients. Merely square-integrable functions need not have pointwise convergence.

For the [Haar wavelet](../../../../../haar-wavelet.md), use the cell convention $I_{j,k}=(k2^{-j},(k+1)2^{-j}]$ and let $I_j(x)$ be the unique such interval containing $x$. The [Haar scaling functions](../../../../../haar-scaling-function.md) are $2^{j/2}\mathbf1_{I_{j,k}}$, so the [Haar projection](../../../../../haar-projection.md) is

$$
K_jf(x)=2^j\int_{I_j(x)}f(t)\,dt.
$$

For a merely locally integrable function this cell-average formula remains defined, even if a global $L^2$ orthogonal projection is unavailable. If $\|f'\|_\infty=L$, the [mean value theorem](../../../../../mean-value-theorem.md) gives [Lipschitz continuity](../../../../../lipschitz-continuity.md) and, since $|t-x|\le2^{-j}$ on the cell,

$$
|K_jf(x)-f(x)|\le2^j\int_{I_j(x)}L|t-x|\,dt\le L2^{-j}.
$$

Thus the requested bound holds with $\boxed{c=\|f'\|_\infty}$, by the [Haar projection error for a Lipschitz function](../../../../../haar-projection-error-for-a-lipschitz-function.md).

To estimate a density, replace each scaling or wavelet coefficient $\int f\phi_{j,k}$ or $\int f\psi_{j,k}$ by the sample average of that basis function. The finite-resolution [Haar density estimator](../../../../../haar-density-estimator.md) is therefore

$$
\widehat f_j^W(x)=\sum_k\left(\frac1n\sum_{i=1}^n\phi_{j,k}(X_i)\right)\phi_{j,k}(x)
=\frac{2^j}{n}\sum_{i=1}^n\mathbf1_{I_j(x)}(X_i).
$$

It is the [histogram](../../../../../histogram.md) on the dyadic cells, is nonnegative, and integrates to one. Its expectation is $K_jf(x)$. A density with bounded derivative is bounded: the [Lipschitz density height bound](../../../../../lipschitz-density-height-bound.md) gives $f(x)^2\le L$ by integrating the triangular lower envelope $(f(x)-L|t-x|)_+$. The case $L=0$ cannot be a probability density on the whole real line. Hence $B=\|f\|_\infty<\infty$.

The cell probability is $p_j(x)=\int_{I_j(x)}f\le B2^{-j}$. The sample count has a [binomial distribution](../../../../../binomial-distribution.md), so

$$
\operatorname{Var}(\widehat f_j^W(x))=\frac{2^{2j}}n p_j(x)(1-p_j(x))\le\frac{B2^j}n.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) bounds the mean centered absolute deviation by the square root of this variance. Adding the projection bias gives

$$
\mathbb E|\widehat f_j^W(x)-f(x)|\le L2^{-j}+\sqrt{\frac{B2^j}n}.
$$

Choose $j_n=\lfloor(\log_2n)/3\rfloor$, so $2^{j_n}\asymp n^{1/3}$. The two terms have the same order, and

$$
\boxed{\mathbb E|\widehat f_{j_n}^W(x)-f(x)|=O(n^{-1/3}).}
$$

This is a [bias-variance tradeoff](../../../../../bias-variance-tradeoff.md): refining the cells decreases the averaging bias but increases the sampling variance.

<a id="3/image-haar-projections-of-the-standard-normal-density-at-three-resolutions"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33-haar-projections.png)

**[Figure 1](#3/image-haar-projections-of-the-standard-normal-density-at-three-resolutions). Haar projections of the standard normal density at three resolutions**.

The [Haar projection](../../../../../haar-projection.md) averages this [normal distribution](../../../../../normal-distribution.md) density on each cell; the finer cells follow its variation more closely. A [Haar density estimator](../../../../../haar-density-estimator.md) replaces these exact cell probabilities by empirical frequencies and therefore also introduces sampling noise.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
