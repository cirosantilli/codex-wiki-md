<h1 id="o/2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Centering gives $\sum_i z_i=0$, and hence

$$
X^{\mathsf T}X=\begin{pmatrix}n&0\\0&\sum_i z_i^2\end{pmatrix}.
$$

The least-squares [covariance](../../../../../../covariance.md) formula from part (a) therefore gives

$$
\boxed{\operatorname{Var}\begin{pmatrix}\widehat\alpha\\\widehat\beta\end{pmatrix}
=\sigma^2\begin{pmatrix}1/n&0\\0&1/\sum_i(e^{-t_i}-c)^2\end{pmatrix}.}
$$

Explicitly $\widehat\alpha=\overline Y$ and $\widehat\beta=\sum_i z_iY_i/\sum_i z_i^2$. Their zero [covariance](../../../../../../covariance.md) follows directly from the centered predictor, and their joint normality additionally makes them independent.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [O](../../../../o.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options I course of the University of Oxford](../../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
