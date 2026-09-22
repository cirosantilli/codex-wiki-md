<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $v=\sigma^2>0$, $d_k=k+1$, and $S_k(a)=\|y-X_ka\|^2$. Under the standard interpretation that the two stated priors are independent, multiply the normal likelihood by the normal coefficient prior and the [inverse-gamma distribution](../../../../../../../inverse-gamma-distribution.md) density. The [independent normal and inverse-gamma regression priors](../../../../../../../independent-normal-and-inverse-gamma-regression-priors.md) give

$$
\boxed{\pi(a_k,v\mid x,y)\propto
v^{-(\alpha+1+n/2)}
\exp\left[-\frac{\beta+S_k(a_k)/2}{v}
-\frac12(a_k-\mu_k)^T\Sigma_k^{-1}(a_k-\mu_k)\right],\quad v>0.}
$$

For a fixed model the determinant and Gaussian normalizing constants are independent of $a_k,v$ and may be omitted here; $\Sigma_k$ is assumed [positive-definite](../../../../../../../positive-definite-bilinear-form.md). The coefficient prior is not scaled by $v$, so replacing its precision by $\Sigma_k^{-1}/v$ would describe a different prior.

For an additional check, completing the coefficient square and reading the [variance](../../../../../../../variance-split.md) kernel give the full conditional distributions

$$
a_k\mid v,x,y\sim N(m_k,V_k),\quad
V_k=(X_k^TX_k/v+\Sigma_k^{-1})^{-1},\quad
m_k=V_k(X_k^Ty/v+\Sigma_k^{-1}\mu_k),
$$

and

$$
v\mid a_k,x,y\sim\operatorname{InvGamma}(\alpha+n/2,\beta+S_k(a_k)/2).
$$

Marginal priors alone would not determine their joint prior without the independence assumption. The front-page inverse-gamma mean has a typographical error: this density has mean $\beta/(\alpha-1)$ when $\alpha>1$, not a denominator $\alpha+1$. The density itself, used in the posterior calculation, fixes the correct parameterization.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
