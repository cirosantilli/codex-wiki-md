<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Put $\Delta=\Theta-\Sigma$ and let $\beta$ lie in the compatibility cone. Then

$$
|\beta^T\Delta\beta|
\leq\|\Delta\|_\infty\|\beta\|_1^2
\leq16\|\Delta\|_\infty\|\beta_S\|_1^2
\leq\frac{\phi_\Sigma^2(S)}{2|S|}\|\beta_S\|_1^2.
$$

Subtracting this from the defining lower bound for $\beta^T\Sigma\beta$ and taking the infimum gives the [stability of a compatibility constant under entrywise perturbation](../../../../../stability-of-a-compatibility-constant-under-entrywise-perturbation.md):

$$
\boxed{\phi_\Theta^2(S)\geq\frac12\phi_\Sigma^2(S).}
$$

A centered random variable $W$ is a [sub-Gaussian random variable](../../../../../sub-gaussian-distribution.md) with parameter $\sigma$ when

$$
\mathbb E e^{tW}\leq e^{\sigma^2t^2/2}
\qquad(t\in\mathbb R).
$$

The [Chernoff bound](../../../../../chernoff-bound.md) gives $\mathbb P(W>t)\leq e^{-t^2/(2\sigma^2)}$.

For fixed $j,k$, the variables

$$
W_i=X_{ij}X_{ik}-\Sigma_{jk}
$$

are independent, centered, and lie in $[-2,2]$, hence are sub-Gaussian with parameter $2$. Their mean is sub-Gaussian with parameter $2/\sqrt n$, so

$$
\mathbb P(|\widehat\Sigma_{jk}-\Sigma_{jk}|>t)
\leq2e^{-nt^2/8}.
$$

A [union bound](../../../../../boole-s-inequality.md) over at most $p^2$ pairs with $t=4\sqrt{2\log(p)/n}$ yields

$$
\boxed{\mathbb P\left(
\|\widehat\Sigma-\Sigma\|_\infty>
4\sqrt{\frac{2\log p}{n}}
\right)\leq\frac2{p^2}.}
$$

The minimum-eigenvalue bound and [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) imply

$$
\beta^T\Sigma\beta\geq c_{\min}\|\beta\|_2^2
\geq\frac{c_{\min}}{|S|}\|\beta_S\|_1^2,
$$

so $\phi_\Sigma^2(S)\geq c_{\min}$. A sufficient uniform condition is

$$
\boxed{c_{\min}\geq128s\sqrt{\frac{2\log p}{n}}.}
$$

Indeed, on the concentration event the entrywise error is at most $c_{\min}/(32s)\leq\phi_\Sigma^2(S)/(32|S|)$ for every $0<|S|\leq s$. The perturbation result then gives $\phi_{\widehat\Sigma}^2(S)\geq c_{\min}/2$ simultaneously, with probability at least $1-2p^{-2}$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
