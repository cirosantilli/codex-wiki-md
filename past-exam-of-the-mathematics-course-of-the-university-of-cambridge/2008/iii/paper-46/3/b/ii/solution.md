<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $X=\sum_i x_i>0$ and $d=\sum_i v_i$. The exponential [survival likelihood](../../../../../../../survival-likelihood.md) has $\ell(\lambda)=d\log\lambda-\lambda X$. Its score is $d/\lambda-X$, and for $d>0$ its second derivative is $-d/\lambda^2<0$. Thus the [exponential-rate estimation from censored exposure](../../../../../../../exponential-rate-estimation-from-censored-exposure.md) gives

$$
\boxed{\widehat\lambda=\frac dX.}
$$

All observation times, including censoring times, belong in $X$. If $d=0$, the [likelihood](../../../../../../../likelihood-function.md) decreases with positive $\lambda$ and has its supremum as $\lambda\downarrow0$; under the stated strict positivity constraint there is no interior maximum.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 46](../../../../paper-46-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
