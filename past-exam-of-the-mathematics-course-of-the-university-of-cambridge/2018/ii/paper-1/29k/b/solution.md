<h1 id="29k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The expectation is

$$
\mathbb E_\theta[\widehat\theta_w]
=w_{AA}(1-\theta)^2+w_{BB}\theta^2
+2w_{AB}\theta(1-\theta).
$$

For this polynomial to equal $\theta$ for every $\theta\in(0,1)$, comparison of its constant, linear, and quadratic coefficients gives

$$
w_{AA}=0,
\qquad 2w_{AB}=1,
\qquad w_{BB}-2w_{AB}=0.
$$

Thus the unique choice is

$$
\boxed{\ w^*=(0,1,1/2),
\qquad
\widehat\theta_{w^*}=\frac{2n_{BB}+n_{AB}}{2n}.\ }
$$

For fly $i$, let $Z_i$ be half its number of $B$ alleles. Then $Z_i\in\{0,1/2,1\}$, the $Z_i$ are independent and identically distributed,

$$
\mathbb EZ_i=\theta,
\qquad
\operatorname{Var}(Z_i)=\frac{\theta(1-\theta)}2,
$$

and $\widehat\theta_{w^*}=n^{-1}\sum_iZ_i$. The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) gives $\widehat\theta_{w^*}\to\theta$ in probability. Hence **the estimator is unbiased and consistent**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [29K](../../29k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
