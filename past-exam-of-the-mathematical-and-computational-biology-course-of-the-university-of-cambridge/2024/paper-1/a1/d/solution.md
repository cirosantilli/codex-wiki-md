<h1 id="a1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $s=\sum_i\log x_i<0$. The [score function](../../../../../informant-function.md) is

$$
\ell'(\theta)=\frac{N}{\theta+1}+s.
$$

Setting it to zero gives the [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md)

$$
\boxed{\widehat\theta=-\frac{N}{\sum_i\log x_i}-1}.
$$

This lies above $-1$. The [observed Fisher information](../../../../../observed-fisher-information.md) is

$$
\boxed{J(\theta)=-\ell''(\theta)=\frac{N}{(\theta+1)^2}>0}.
$$

Consequently the [log-likelihood](../../../../../log-likelihood.md) is strictly concave throughout its domain. Its stationary point is the unique global maximum, not merely a candidate local maximum. Indeed the [log-likelihood](../../../../../log-likelihood.md) tends to minus infinity as either $\theta\downarrow-1$ or $\theta\to\infty$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [A1](../../a1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
