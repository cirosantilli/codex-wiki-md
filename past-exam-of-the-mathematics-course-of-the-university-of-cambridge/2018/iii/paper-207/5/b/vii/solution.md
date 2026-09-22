<h1 id="5/b/vii/solution">Solution</h1>

↑ **Parent:** [Vii](../vii.md)

Insert the [Breslow estimator](../../../../../../../breslow-estimator.md) into the fitted cumulative intensities and interchange the finite sums:

$$
\begin{aligned}
\sum_{i=1}^n e^{\widehat\beta z_i}\widehat H_0(x_i)
&=\sum_{i=1}^n e^{\widehat\beta z_i}
\sum_{\ell:x_\ell\leq x_i}\frac{v_\ell}{\sum_{j:x_j\geq x_\ell}e^{\widehat\beta z_j}}\\
&=\sum_{\ell=1}^n
\frac{v_\ell\sum_{i:x_i\geq x_\ell}e^{\widehat\beta z_i}}
{\sum_{j:x_j\geq x_\ell}e^{\widehat\beta z_j}}
=\sum_{\ell=1}^n v_\ell.
\end{aligned}
$$

Every observed event contributes exactly one after summing its fitted contribution over its [risk set](../../../../../../../risk-set.md). Therefore

$$
\boxed{\sum_{i=1}^n y_i=\sum_i v_i-\sum_i e^{\widehat\beta z_i}\widehat H_0(x_i)=0.}
$$

This identity is algebraic and holds for any finite coefficient used consistently in the relative hazards and the [Breslow estimator](../../../../../../../breslow-estimator.md); it does not require the [score equation](../../../../../../../score-equation.md) to be solved exactly. It can fail if the [baseline hazard](../../../../../../../baseline-hazard.md) is estimated or smoothed by a different procedure.

## ↑ Ancestors (12)

1. [Vii](../vii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
