<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For observed data $x$ and missing data $z$, let $p_\theta(x,z)$ be the complete-data model. Starting at $\theta^{(0)}$, the [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) alternates

$$
Q(\theta\mid\theta^{(r)})
=\mathbb E_{\theta^{(r)}}[\log p_\theta(x,Z)\mid x],
\qquad
\theta^{(r+1)}\in\operatorname*{arg\,max}_\theta Q(\theta\mid\theta^{(r)}).
$$

The E-step computes the [conditional expectation](../../../../../../conditional-expectation.md) of the complete-data [log-likelihood](../../../../../../log-likelihood.md), using the current parameter for the missing-data [conditional distribution](../../../../../../conditional-distribution.md). The M-step maximizes that expected [log-likelihood](../../../../../../log-likelihood.md) over a new parameter. Maximizing the [likelihood](../../../../../../likelihood-function.md) of imputed [mean](../../../../../../expected-value.md) data is equivalent only when the complete-data [log-likelihood](../../../../../../log-likelihood.md) has the necessary linear dependence on the missing sufficient statistics.

For the monotonicity argument, let $q_r(z)=p_{\theta^{(r)}}(z\mid x)$. [Jensen inequality](../../../../../../jensen-s-inequality.md) gives

$$
\log p_\theta(x)-\log p_{\theta^{(r)}}(x)
=\log\mathbb E_{q_r}\left[\frac{p_\theta(x,Z)}{p_{\theta^{(r)}}(x,Z)}\right]
\geq Q(\theta\mid\theta^{(r)})-Q(\theta^{(r)}\mid\theta^{(r)}).
$$

Therefore an M-step increasing $Q$ cannot decrease the observed-data [likelihood](../../../../../../likelihood-function.md). Standard support and [integrability](../../../../../../integrability.md) conditions are understood. EM need not find a global maximum for a general model; its behavior depends on the objective and starting point.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
