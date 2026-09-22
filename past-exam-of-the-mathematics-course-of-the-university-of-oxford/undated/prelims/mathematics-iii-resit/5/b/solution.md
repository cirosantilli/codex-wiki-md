<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [random variables](../../../../../../random-variable-split.md) with finite [second moments](../../../../../../second-moment.md), their [covariance](../../../../../../covariance.md) is

$$
\boxed{\operatorname{Cov}(X,Y)=\mathbb E[(X-\mathbb EX)(Y-\mathbb EY)].}
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) ensures the product is [integrable](../../../../../../integrability.md). Expand and use [linearity of expectation](../../../../../../linearity-of-expectation.md):

$$
\begin{aligned}
\operatorname{Cov}(X,Y)
&=\mathbb E[XY]-\mathbb E[X]\mathbb E[Y]
-\mathbb E[X]\mathbb E[Y]+\mathbb E[X]\mathbb E[Y]\\
&=\boxed{\mathbb E[XY]-\mathbb E[X]\mathbb E[Y].}
\end{aligned}
$$

The same identity holds whenever the quantities involved exist with sufficient [integrability](../../../../../../integrability.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Mathematics III resit](../../../mathematics-iii-resit-split.md)
4. [Prelims](../../../split.md)
5. [Undated](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
