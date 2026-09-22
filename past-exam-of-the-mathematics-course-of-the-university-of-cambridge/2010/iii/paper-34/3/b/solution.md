<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D_k=\sum_{j:g_j=k}v_j$ be the observed event count and $T_k=\sum_{j:g_j=k}x_j$ the total [person-time](../../../../../../person-time.md) in group $k$. Both groups are present; suppose each has $T_k>0$. The grouped [log-likelihood](../../../../../../log-likelihood.md) is

$$
\ell(\beta^{(0)},\beta^{(1)})=\sum_{k=0}^1\{D_k\log\beta^{(k)}-T_k\beta^{(k)}\}+\text{constant}.
$$

When $D_k>0$, its derivative is $D_k/\beta^{(k)}-T_k$ and its second derivative is $-D_k/(\beta^{(k)})^2<0$. Therefore the [maximum-likelihood estimates](../../../../../../maximum-likelihood-estimator.md) are

$$
\boxed{\widehat\beta^{(k)}=D_k/T_k,\qquad k=0,1.}
$$

Both events and censored observations contribute to $T_k$. If $D_k=0$, the likelihood decreases with the positive rate: its supremum is at the boundary $\beta^{(k)}\downarrow0$, rather than at a finite strictly positive estimate. Writing $D_k/T_k=0$ then describes the closure estimate.

Under the [null hypothesis](../../../../../../null-hypothesis.md) of a common rate, the same maximization gives

$$
\boxed{\widetilde\beta=\frac{D_0+D_1}{T_0+T_1}.}
$$

Let $D=D_0+D_1$ and $T=T_0+T_1$. The maximized linear terms cancel, since $T_k\widehat\beta^{(k)}=D_k$ and $T\widetilde\beta=D$. Thus the [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) uses

$$
\boxed{W=-2\log\Lambda
=2\left[\sum_{k=0}^1D_k\log\frac{D_k}{T_k}-D\log\frac DT\right]
=2\sum_{k=0}^1D_k\log\frac{D_kT}{DT_k}.}
$$

Interpret a zero-event summand by continuity as zero. If $D=0$, both likelihood suprema are equal and $W=0$: no rate comparison is informed by observed events.

Under positive common hazard, [independent censoring](../../../../../../independent-censoring.md) and the usual increasing-information conditions in both groups, [Wilks theorem](../../../../../../wilks-theorem.md) gives $W\Rightarrow\chi_1^2$, because the unrestricted model has two rate parameters and the null has one. Reject for large $W$; at 5%, the usual cutoff is approximately $3.84$. The chi-squared calibration is asymptotic and can be poor with sparse event counts or boundary estimates.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
