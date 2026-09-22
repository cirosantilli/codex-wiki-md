<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The score equation $X^T(\mu-Y)=0$ is independent of $\gamma$, because $\gamma>0$ is only a common factor. Fixing $\phi=1$ or estimating it therefore gives the same [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) $\widehat\beta$.

Under the usual full-rank and regularity conditions,

$$
\widehat\beta
\mathrel{\dot\sim}
N_4\!\left(
\beta,\,
\phi(X^TWX)^{-1}
\right),
$$

with $W$ evaluated consistently at the fitted means. Consequently every standard error from "mod2" is $\sqrt{\widehat\phi}$ times the corresponding standard error computed with dispersion one in "mod1". In particular,

$$
\boxed{\operatorname{SE}_{\rm mod2}(\widehat\beta_{\rm posout})
=\sqrt{0.3103711}\,(0.04556).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
