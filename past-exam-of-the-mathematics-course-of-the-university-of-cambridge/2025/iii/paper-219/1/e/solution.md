<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Differentiating the log-likelihood gives the unique stationary point

$$
\widehat M_0^*=s_1,
\qquad
\widehat{\Delta M}=\frac1G\sum_gs_{2g},
\qquad
\widehat{\mathcal M}=\frac1{N_{\mathrm{SN}}}\sum_is_{3i}.
$$

Its Hessian is diagonal with entries $-1/V_1$, $-G/V_2$, and $-N_{\mathrm{SN}}/\sigma_{\mathrm{SN}}^2$, so it is the unique maximum. The estimators are unbiased and have variances

$$
V_1,
\qquad
\frac{V_2}{G},
\qquad
\frac{\sigma_{\mathrm{SN}}^2}{N_{\mathrm{SN}}},
$$

which equal their [Cramér-Rao lower bounds](../../../../../../cramer-rao-bound.md) because the normal location statistics are efficient.

Since $\theta=M_0^*+\Delta M-\mathcal M$, invariance of the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) gives

$$
\widehat\theta=\widehat M_0^*+\widehat{\Delta M}-\widehat{\mathcal M}.
$$

It is unbiased and normal with variance

$$
\boxed{\sigma_\theta^2
=V_1+\frac{V_2}{G}
+\frac{\sigma_{\mathrm{SN}}^2}{N_{\mathrm{SN}}}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
