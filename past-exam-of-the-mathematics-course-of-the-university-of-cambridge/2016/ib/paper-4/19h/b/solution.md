<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\mathrm{RSS}_1=\sum_i(Y_i-\widehat\alpha-\widehat\beta x_i)^2$ for the unrestricted fit. Under $H_0$, the best slope is still $\widehat\beta$ because the design is centered. Orthogonality of the residuals to the constant vector gives

$$
\mathrm{RSS}_0=\sum_i(Y_i-\widehat\beta x_i)^2=\mathrm{RSS}_1+n\overline Y^2.
$$

At either fitted mean, the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) of variance is $\mathrm{RSS}/n$. The ratio used by the [generalized likelihood-ratio test](../../../../../../generalized-likelihood-ratio-test.md) is consequently

$$
\Lambda=\left(\frac{\mathrm{RSS}_1}{\mathrm{RSS}_0}\right)^{n/2}=\left(1+\frac{T_n^2}{n-2}\right)^{-n/2},\qquad T_n=\frac{\sqrt n\,\overline Y}{\sqrt{\mathrm{RSS}_1/(n-2)}}.
$$

Small likelihood ratios correspond to large $|T_n|$. Under $H_0$, part (a) gives independent $\sqrt n\,\overline Y/\sigma\sim N(0,1)$ and $\mathrm{RSS}_1/\sigma^2\sim\chi^2_{n-2}$. Thus $T_n$ has the [Student's t-distribution](../../../../../../student-s-t-distribution.md) with $n-2$ degrees of freedom. **The exact size-5% critical region is**

$$
\boxed{|T_n|>t_{n-2,\,0.975},}
$$

where $t_{\nu,0.975}$ is the 97.5th percentile of that distribution. The denominator uses the unbiased residual variance estimate, not the likelihood variance denominator $n$.

Under an alternative, the same statistic has the representation

$$
T_n=\frac{Z+\sqrt n\,\alpha/\sigma}{\sqrt{W/(n-2)}},\qquad Z\sim N(0,1),\quad W\sim\chi^2_{n-2},\quad Z\perp W.
$$

The joint law of $Z,W$ is parameter-free, and $\beta$ has disappeared. Therefore

$$
\boxed{w(\alpha,\beta,\sigma^2)=g(\alpha/\sigma),}
$$

where $g(d)=\mathbb P(|(Z+\sqrt n d)/\sqrt{W/(n-2)}|>t_{n-2,0.975})$. This is also the [noncentral t-distribution](../../../../../../noncentral-t-distribution.md) description of the power. As explained in part (a), an exact residual-based test requires $n>2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
