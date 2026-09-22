<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Average the covariate over its possible event subjects using the conditional [probabilities](../../../../../../probability.md) from part (a). Define the risk-weighted sums

$$
S_r(t,\beta)=\sum_{i\in R(t)}z_i^r e^{\beta z_i},\qquad r=0,1,2,
$$

with $z_i^0=1$. Then

$$
\boxed{\overline z(t^*,\beta)=\frac{S_1(t^*,\beta)}{S_0(t^*,\beta)}
=\frac{\sum_{i\in R(t^*)}z_i e^{\beta z_i}}{\sum_{i\in R(t^*)}e^{\beta z_i}}.}
$$

This is the mean covariate of the next event subject, conditional on the current [risk set](../../../../../../risk-set.md) and an event. It is generally not the unweighted average over the original sample. For $\beta=0$ it reduces to the unweighted current risk-set mean.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
