<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The alternative effective count is

$$
\boxed{p_V=\frac12\operatorname{Var}\{D(\theta)\mid y\}.}
$$

Under the locally flat-prior approximation, the constant $D(\widehat\theta)$ contributes no [variance](../../../../../../variance-split.md), and the remaining [chi-squared distribution](../../../../../../chi-squared-distribution.md) term has [variance](../../../../../../variance-split.md) $2p$. Hence $p_V\approx p$, the same calibration as the usual [effective parameter count in DIC](../../../../../../effective-parameter-count-in-dic.md). It can be estimated by half the sample variance of deviance draws, without evaluating deviance at a parameter average.

This is a calibrated alternative, not a general identity with $p_D$. For example, with a quadratic deviance and a [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) posterior of mean $m$ and covariance $\Sigma$, putting $b=m-\widehat\theta$ gives

$$
p_V=\operatorname{tr}\{(J\Sigma)^2\}+2b^TJ\Sigma Jb,
\qquad p_D=\operatorname{tr}(J\Sigma).
$$

They agree when $b=0$ and $\Sigma=J^{-1}$, but informative priors can change both the covariance and the displacement of the posterior mean. Their equality should therefore not be assumed outside the stated regime.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
