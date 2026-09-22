<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $I_0=\{i:y_i=0\}$ and $I_+=\{i:y_i>0\}$. Under the proposed [zero-inflated negative binomial model](../../../../../../zero-inflated-negative-binomial-model.md), [independence](../../../../../../independent-random-variables.md) gives the [likelihood function](../../../../../../likelihood-function.md)

$$
\boxed{L(\pi,\beta;r)=\prod_{i\in I_0}\left[\pi+(1-\pi)\left(\frac{r}{r+e^{x_i^T\beta}}\right)^r\right]\prod_{i\in I_+}(1-\pi)f_{\rm NB}(y_i;r,e^{x_i^T\beta}).}
$$

The positive-count factor uses the ordinary, untruncated [negative binomial distribution](../../../../../../negative-binomial-distribution.md). With $f_i=f_{\rm NB}(y_i;r,\lambda_i)$, the [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell=\sum_{i\in I_0}\log[\pi+(1-\pi)f_i]+\sum_{i\in I_+}[\log(1-\pi)+\log f_i].
$$

For latent indicators $a_i$, the complete-data [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell_c=\sum_i\{a_i\log\pi+(1-a_i)[\log(1-\pi)+\log f_i]\},
$$

where $a_i=1$ is allowed only when $y_i=0$. This separation is what makes the [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) convenient.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
