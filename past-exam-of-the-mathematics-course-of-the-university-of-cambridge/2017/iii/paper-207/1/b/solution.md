<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\widehat\delta_D$ and $\widehat\delta_I$ be [independent](../../../../../../independent-random-variables.md), approximately unbiased estimates of one consistent treatment effect, with [variances](../../../../../../variance-split.md) $v_D,v_I>0$. The [inverse-variance weighted mean](../../../../../../inverse-variance-weighted-mean.md) gives

$$
\boxed{\widehat\delta=\frac{\widehat\delta_D/v_D+\widehat\delta_I/v_I}{1/v_D+1/v_I},\qquad \operatorname{Var}(\widehat\delta)=\left(\frac1{v_D}+\frac1{v_I}\right)^{-1}.}
$$

Indeed, weights $w,1-w$ give [variance](../../../../../../variance-split.md) $w^2v_D+(1-w)^2v_I$; differentiating gives $w=v_I/(v_D+v_I)$, the weight on the direct estimate. Here the three displayed trials give $\widehat\delta_D=-1.33$, $v_D=0.04$, and hence $\widehat\delta\simeq-1.3203$ with [variance](../../../../../../variance-split.md) $0.03448$. This numerical pooling uses the displayed evidence, not the unavailable data from all twelve trials. A shared study or shared control would introduce [covariance](../../../../../../covariance.md), requiring the corresponding correlated-estimator formula; inconsistency would invalidate the common-effect interpretation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
