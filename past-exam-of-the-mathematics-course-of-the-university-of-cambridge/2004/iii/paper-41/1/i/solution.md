<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\Lambda=\sum_{i=1}^m\lambda_i$. For $\Lambda>0$, the resulting [compound Poisson distribution](../../../../../../compound-poisson-distribution.md) has

$$
\boxed{\text{count parameter }\Lambda,\qquad
F(x)=\sum_{i=1}^m\frac{\lambda_i}{\Lambda}F_i(x).}
$$

Thus the merged [claim size](../../../../../../claim-size.md) [probability distribution](../../../../../../probability-distribution.md) is a rate-weighted [mixture distribution](../../../../../../mixture-distribution.md), not an equally weighted [mixture distribution](../../../../../../mixture-distribution.md) unless the rates agree.

To prove this without any [moment-generating function](../../../../../../moment-generating-function.md) assumption, let $\chi_i(t)$ be the [characteristic function](../../../../../../characteristic-function.md) of a claim of type $i$. Conditioning on its [Poisson distribution](../../../../../../poisson-distribution.md) count gives

$$
\mathbb Ee^{itS_i}=\exp\{\lambda_i(\chi_i(t)-1)\}.
$$

[Independence](../../../../../../independent-random-variables.md) of the aggregate risks therefore gives

$$
\mathbb Ee^{itS}
=\prod_i\exp\{\lambda_i(\chi_i(t)-1)\}
=\exp\left\{\Lambda\left(\sum_i\frac{\lambda_i}{\Lambda}\chi_i(t)-1\right)\right\}.
$$

The weighted [characteristic function](../../../../../../characteristic-function.md) inside is precisely that of the displayed [mixture distribution](../../../../../../mixture-distribution.md). This is the transform of a sum of [independent](../../../../../../independent-random-variables.md) claims with [independent](../../../../../../independent-random-variables.md) count $\operatorname{Pois}(\Lambda)$, proving the claim by uniqueness of [characteristic functions](../../../../../../characteristic-function.md). This is [Poisson superposition of insurance portfolios](../../../../../../poisson-superposition-of-insurance-portfolios.md). If $\Lambda=0$, all risks make no claims [almost surely](../../../../../../almost-sure-convergence.md) and $S=0$; the severity law is then irrelevant.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
