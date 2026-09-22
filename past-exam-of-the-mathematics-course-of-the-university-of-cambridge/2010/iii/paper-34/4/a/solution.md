<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Keep the [counting process](../../../../../../counting-process.md) and [at-risk process](../../../../../../at-risk-process.md) notation from the introductory derivation. Because the individual hazards add, the aggregate conditional intensity is

$$
\lambda(t)=\sum_iY_i(t)h_{0i}(t)+Y(t)h_1(t).
$$

The known individual contributions must be averaged over the current [risk set](../../../../../../risk-set.md), rather than over the original cohort. Define

$$
\overline h_0(t)=\frac{\sum_iY_i(t)h_{0i}(t)}{Y(t)}\qquad(Y(t)>0).
$$

Then $dN(t)/Y(t)$ estimates $\{\overline h_0(t)+h_1(t)\}dt$. Subtract the known average contribution to obtain the [offset-adjusted cumulative hazard estimator](../../../../../../offset-adjusted-cumulative-hazard-estimator.md)

$$
\boxed{\widehat H_1(t)
=\sum_{a_j\leq t}\frac1{r_j}
-\int_0^t\mathbf1_{\{Y(u)>0\}}\frac{\sum_iY_i(u)h_{0i}(u)}{Y(u)}\,du.}
$$

Take the quotient to be zero when $Y=0$. If $M(t)=N(t)-\int_0^t\lambda(u)du$, direct substitution gives

$$
\widehat H_1(t)
=\int_0^t\mathbf1_{\{Y(u)>0\}}h_1(u)du
+\int_0^t\frac{\mathbf1_{\{Y(u)>0\}}}{Y(u)}\,dM(u).
$$

This establishes the target and the mean-zero estimation noise, under the usual integrability conditions. It estimates $H_1(t)$ while there is a nonempty [risk set](../../../../../../risk-set.md); no data identify its continuation after follow-up has ended. With common known $h_{0i}=h_0$ and individuals at risk throughout $[0,t]$, it reduces to $\widehat H_1(t)=\widehat H(t)-H_0(t)$.

The estimate may decrease between events because the known offset is subtracted continuously. That is not an algebraic error: it is an unconstrained estimating-equation estimator, not automatically a nonnegative monotone cumulative hazard estimate. If such shape constraints are imposed, the fitting procedure must explicitly account for them. The working hazard model itself must satisfy $h_{0i}+h_1\geq0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
