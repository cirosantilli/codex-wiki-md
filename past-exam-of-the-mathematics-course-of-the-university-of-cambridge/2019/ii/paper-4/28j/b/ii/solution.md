<h1 id="28j/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put

$$
\sigma_h^2=\operatorname{Var}_{\theta_0}(h(X)).
$$

The [central limit theorem](../../../../../../../central-limit-theorem.md) gives $\sqrt n(\widehat\mu_n-\mu(\theta_0))\Rightarrow N(0,\sigma_h^2)$. Provided $\mu'(\theta_0)\ne0$, the [delta method](../../../../../../../delta-method.md) applied to $\mu^{-1}$ yields

$$
\boxed{\sqrt n(\widehat\theta_n-\theta_0)
\xrightarrow d
N\left(0,\frac{\sigma_h^2}{\mu'(\theta_0)^2}\right).}
$$

Strict monotonicity alone does not exclude $\mu'(\theta_0)=0$; in that exceptional case this root-$n$ limit need not hold and higher-order analysis is required.

One does **not** necessarily have $\operatorname{Var}(\widehat\theta_n)\geq[nI(\theta_0)]^{-1}$ for every $n$, because $\widehat\theta_n$ need not be unbiased. The [Cramér-Rao bound](../../../../../../../cramer-rao-bound.md) for an estimator with bias $B_n(\theta)$ is instead

$$
\operatorname{Var}_\theta(\widehat\theta_n)
\geq\frac{(1+B_n'(\theta))^2}{nI(\theta)}
$$

under the corresponding regularity assumptions.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [28J](../../../28j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
