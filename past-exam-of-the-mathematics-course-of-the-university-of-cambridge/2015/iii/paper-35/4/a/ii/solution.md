<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An exact observed event contributes **its event-time density**:

$$
\boxed{L_i=f(x_i)=-F'(x_i).}
$$

For [exponential-rate estimation from censored exposure](../../../../../../../exponential-rate-estimation-from-censored-exposure.md), the event-model [survival likelihood](../../../../../../../survival-likelihood.md) under [independent censoring](../../../../../../../independent-censoring.md) is $\prod_i f(x_i)^{v_i}F(x_i)^{1-v_i}$. For the [exponential distribution](../../../../../../../exponential-distribution.md), put $d=\sum_i v_i$ and $X=\sum_i x_i$. Then

$$
L(\theta)=\theta^d e^{-\theta X},\qquad
\ell(\theta)=d\log\theta-\theta X+\text{constant}.
$$

If $d>0$ and $X>0$, $\ell'(\theta)=d/\theta-X$ vanishes at

$$
\boxed{\widehat\theta=\frac{d}{X}.}
$$

The second derivative $-d/\theta^2$ is strictly negative, so this is the unique global [maximum-likelihood estimate](../../../../../../../maximum-likelihood-estimator.md). The likelihood also tends to zero at both ends of the positive parameter range. If $d=0$ and $X>0$, the likelihood decreases on $\theta>0$; its supremum is at $\theta\downarrow0$, with no attained positive estimate. Thus every censored time belongs in the exposure denominator.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
