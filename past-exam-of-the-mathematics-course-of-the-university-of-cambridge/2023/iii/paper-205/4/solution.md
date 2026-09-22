<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A centered [random variable](../../../../../random-variable-split.md) $X$ is [sub-Gaussian](../../../../../sub-gaussian-distribution.md) with parameter $a>0$ when

$$
\mathbb E e^{tX}\leq e^{a^2t^2/2}
$$

for every $t\in\mathbb R$.

The [Bernstein concentration inequality for products of sub-Gaussian variables](../../../../../bernstein-concentration-inequality-for-products-of-sub-gaussian-variables.md) quoted in the course says that if each coordinate of the identically distributed pairs $(U_i,V_i)$ is sub-Gaussian with parameter $\sigma/4$, then

$$
\mathbb P\!\left(\left|\frac1n\sum_{i=1}^n
\{U_iV_i-\mathbb E(U_iV_i)\}\right|\geq t\right)
\leq2\exp\!\left(-\frac{2nt^2}{\sigma^2(\sigma^2+t)}\right).
$$

Since $U^TV=\sum_iU_iV_i$, this is the required bound. It follows by observing that a product of sub-Gaussian variables is [sub-exponential](../../../../../subexponential-distribution-light-tailed.md) and applying [Bernstein's inequality](../../../../../bernstein-inequalities-probability-theory.md) to the independent centered products.

For any vector $\delta$ admissible in the definition of $\phi_\Sigma^2$, one has $\|\delta\|_1\leq4$. The [entrywise maximum norm](../../../../../entrywise-maximum-norm.md) bound therefore implies

$$
|\delta^T(\Theta-\Sigma)\delta|
\leq\max_{j,k}|\Theta_{jk}-\Sigma_{jk}|\,\|\delta\|_1^2
\leq\frac{\phi_\Sigma^2}{2s}.
$$

By the definition of the [compatibility constant](../../../../../compatibility-constant.md), $\delta^T\Sigma\delta\geq\phi_\Sigma^2/s$, and hence

$$
\delta^T\Theta\delta\geq\frac{\phi_\Sigma^2}{2s}.
$$

Taking the infimum proves $\phi_\Theta^2\geq\phi_\Sigma^2/2$. This is the [stability of a compatibility constant under entrywise perturbation](../../../../../stability-of-a-compatibility-constant-under-entrywise-perturbation.md).

Put $C=X^TX/n$. Applying the product concentration bound with the stated $t$ and using $t\leq\sigma^2/3$ gives, for every $j,k$,

$$
\mathbb P(|C_{jk}-\Sigma_{jk}|>t)
\leq2e^{-3\log(p+1)}=\frac2{(p+1)^3}.
$$

There are $p(p+1)/2$ distinct entries in the symmetric matrix, so the [union bound](../../../../../boole-s-inequality.md) shows that the event

$$
\mathcal E=\left\{\max_{j,k}|C_{jk}-\Sigma_{jk}|\leq t\right\}
$$

has probability at least $1-p/(p+1)^2\geq p/(p+1)$.

On $\mathcal E$, $|C_{jj}-1|\leq t$. Since $|\Sigma_{jk}|\leq1$ by [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md), normalization of the sample columns gives

$$
|\widehat\Sigma_{jk}-\Sigma_{jk}|
=\left|\frac{C_{jk}}{\sqrt{C_{jj}C_{kk}}}-\Sigma_{jk}\right|
\leq\frac{2t}{1-t}.
$$

Choosing one coordinate of $S$ in the infimum shows $\phi_\Sigma^2\leq s$, so the assumed bound on $t$ is below one and, more precisely,

$$
t\leq\frac{\phi_\Sigma^2}{64s+\phi_\Sigma^2}
\quad\Longrightarrow\quad
\frac{2t}{1-t}\leq\frac{\phi_\Sigma^2}{32s}.
$$

The perturbation result now gives $\phi_{\widehat\Sigma}^2\geq\phi_\Sigma^2/2$ throughout $\mathcal E$, and therefore

$$
\boxed{\mathbb P(\phi_{\widehat\Sigma}^2\geq\phi_\Sigma^2/2)\geq\frac p{p+1}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
