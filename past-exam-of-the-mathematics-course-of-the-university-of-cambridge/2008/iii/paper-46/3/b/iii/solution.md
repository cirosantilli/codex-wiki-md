<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $g_i=G_i'(x_i)$, $X=\sum_i x_i$, $d=\sum_i v_i$ and $A=\sum_i v_i g_i$. Then $h_i(x_i)=\lambda+g_i$ and

$$
\ell(\lambda)=\sum_i v_i\log(\lambda+g_i)-\lambda X-\sum_iG_i(x_i),\qquad
U(\lambda)=\sum_i\frac{v_i}{\lambda+g_i}-X.
$$

The integrated offsets are known and enter only as constants in estimation of $\lambda$. Let $\lambda_0=d/X$ and assume $d>0$ and every $g_i$ at an event is small compared with $\lambda_0$. Expanding the score gives

$$
U(\lambda)=\frac d\lambda-\frac A{\lambda^2}-X
+O\left(\frac{\sum_i v_i g_i^2}{\lambda^3}\right).
$$

Now write $\lambda=\lambda_0+\delta$ and retain first-order terms in $g_i,\delta$. Since $d/\lambda_0=X$, the equation becomes $-d\delta/\lambda_0^2-A/\lambda_0^2=0$. Therefore the [exponential rate with a small known additive hazard](../../../../../../../exponential-rate-with-a-small-known-additive-hazard.md) estimate is

$$
\boxed{\widehat\lambda\simeq\frac dX-\frac1d\sum_i v_iG_i'(x_i).}
$$

The correction is negative: some event risk is already supplied by the known additive [hazards](../../../../../../../hazard-function.md). As a check, if every $g_i=g$, the score equation gives the exact positive interior estimate $d/X-g$. The approximation is intended for small offsets and a positive interior solution; a negative approximation or no observed events requires handling the boundary rather than reporting a negative rate.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
