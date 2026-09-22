<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The joint [likelihood ratio](../../../../likelihood-ratio.md) in favor of the alternative is

$$
\frac{L_3}{L_2}=\left(\frac32\right)^n\prod_i x_i.
$$

It is increasing in the product, so the [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) rejects for large product, equivalently small $S=-\sum_i\log x_i$. Under $H_0$, the transformation $Z_i=-\log X_i$ gives

$$
\mathbb P_0(Z_i>z)=\mathbb P_0(X_i<e^{-z})=e^{-2z},\qquad z\geq0.
$$

Therefore the $Z_i$ are [independent](../../../../independent-random-variables.md) [exponential random variables](../../../../exponential-distribution.md) of rate two, $S\sim\operatorname{Gamma}(n,\text{rate }2)$, and $4S\sim\chi_{2n}^2$. An exact size-$\alpha$ [critical region](../../../../rejection-region.md) is

$$
\boxed{S\leq c_\alpha},\qquad\boxed{F_{\chi_{2n}^2}(4c_\alpha)=\alpha}.
$$

Equivalently, reject when the [geometric mean](../../../../geometric-mean.md) satisfies $g\geq e^{-c_\alpha/n}$. The boundary distribution is continuous, so no randomization is needed here.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
