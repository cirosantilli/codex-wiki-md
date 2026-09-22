<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

All moments below are under the proper [posterior distribution](../../../../../../bayesian-posterior.md) of part (b). Write the known [covariance matrix](../../../../../../covariance-matrix.md) in block form

$$
\operatorname{Cov}\begin{pmatrix}h(\beta)\\g(\beta)\end{pmatrix}
=\begin{pmatrix}v&c^T\\c&S\end{pmatrix},\qquad
v=\operatorname{Var}(h),\quad c=\operatorname{Cov}(g,h),\quad S=\operatorname{Cov}(g).
$$

The score covariance $S$ is positive definite in this model. Indeed, a further integration by parts gives $\mathbb E[g(\beta)\beta^T]=-I_p$. If $a^TSa=0$, then $a^Tg=0$ almost surely, because $\mathbb E[g]=0$. Multiplying by $a^T\beta$ would give $0=-\|a\|^2$, so $a=0$.

For a fixed coefficient vector $a$, the [control variate](../../../../../../control-variates.md) summand has [variance](../../../../../../variance-split.md)

$$
\begin{aligned}
\operatorname{Var}(h-a^Tg)
&=v-2a^Tc+a^TSa\\
&=v-c^TS^{-1}c+(a-S^{-1}c)^TS(a-S^{-1}c).
\end{aligned}
$$

Thus the unique minimum is attained at $a_*=S^{-1}c$, giving

$$
\boxed{\widehat\mu_{\mathrm{cv}}=\frac1N\sum_{j=1}^N\left[h(\beta^{(j)})-c^TS^{-1}g(\beta^{(j)})\right],\qquad
\operatorname{Var}(\widehat\mu_{\mathrm{cv}})=\frac{v-c^TS^{-1}c}{N}\leq\frac vN.}
$$

The coefficient is fixed because the covariance is assumed known, and the [posterior score control variate](../../../../../../posterior-score-control-variate.md) has mean zero, so this estimator remains unbiased.

We can identify exactly when the improvement is strict. Integration by parts with the bounded smooth function $h$ gives

$$
c=\mathbb E[g h]=-\mathbb E[\nabla h]
=-x_{\mathrm{test}}\,\mathbb E[\phi(x_{\mathrm{test}}^T\beta)].
$$

The scalar expectation is strictly positive. Therefore $c\ne0$ whenever $x_{\mathrm{test}}\ne0$, and positive definiteness gives a strictly smaller variance in that case. If $x_{\mathrm{test}}=0$, $h\equiv1/2$ and both estimators already have variance zero. The printed request for a smaller variance therefore needs this nondegeneracy qualification; a non-increasing variance always holds.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
