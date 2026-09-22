<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If a department has population $P$, $C_{
m pers}$ crimes against persons and $C_{
m prop}$ crimes against property, cancellation of the common numerator gives

$$
\boxed{y=\frac{P/C_{\rm pers}}{P/C_{\rm prop}}=\frac{C_{\rm prop}}{C_{\rm pers}}.}
$$

Thus $y$ is a property-to-person crime count ratio, not its reciprocal. Both counts must be positive for the printed ratio to be defined.

For the reconstructed 85-row data, fit a [normal linear model](../../../../../../normal-linear-model.md) for the [Box–Cox transformation](../../../../../../box-cox-transformation.md) $T_\lambda(y)$, including four region contrasts plus Literacy, Donations and Wealth. With $z_i(\lambda)=(y_i^\lambda-1)/\lambda$ and $z_i(0)=\ln y_i$, the [profile likelihood](../../../../../../profile-likelihood.md), up to constants, is

$$
\ell_p(\lambda)=-\frac{85}{2}\ln\left[\frac{\operatorname{RSS}(\lambda)}{85}\right]
+(\lambda-1)\sum_i\ln y_i.
$$

The second term is the transformation's [Jacobian determinant](../../../../../../jacobian-determinant.md); omitting it would incorrectly compare different response scales. Maximization gives $\widehat\lambda=0.143$, with approximate 95% [likelihood-ratio confidence interval](../../../../../../likelihood-ratio-confidence-interval.md) $[-0.120,0.406]$. The [logarithmic transformation](../../../../../../logarithmic-transformation.md) is inside this interval, whereas the raw-scale choice $\lambda=1$ is far outside: the twice-log-likelihood drops at zero and one are $1.14$ and $39.54$, respectively. A log-response model is therefore a simple supported choice.

In the full log model, partial [F-tests](../../../../../../f-test.md) give $F_{4,77}=13.15$ for Region ($p=3.3\times10^{-8}$), $F_{1,77}=27.99$ for Wealth ($p=1.1\times10^{-6}$), and $p=0.786,0.682$ for Literacy and Donations. Dropping Literacy and Donations together gives $F_{2,77}=0.109$ and $p=0.897$. A parsimonious final [normal linear model](../../../../../../normal-linear-model.md), with C as reference and $W=\mathrm{Wealth}/10$, is

$$
\boxed{\widehat{\ln y}=1.2956+0.07794\mathbf1_E+0.31846\mathbf1_N
-0.57482\mathbf1_S+0.19198\mathbf1_W-0.08539W.}
$$

The standard errors in that order are $0.1056,0.1105,0.1158,0.1102,0.1104,0.01539$; residual standard deviation is $0.3212$ on 79 degrees of freedom and $R^2=0.626$. Use residual-versus-fitted and [quantile-quantile plots](../../../../../../q-q-plot.md), influence diagnostics and checks for remaining curvature to assess the working Gaussian model; the small [p-values](../../../../../../p-value.md) alone do not validate its assumptions.

Holding Region fixed, worsening wealth rank by ten positions multiplies the fitted conditional median ratio by $e^{-0.08539}=0.918$. Relative to C at the same wealth rank, the fitted median multipliers are $1.081$ for E, $1.375$ for N, $0.563$ for S and $1.212$ for W. **Region and wealth rank explain much of the variation; Literacy and Donations add little once those terms are included.** These are associations in the reconstructed dataset. Back-transforming the fitted log mean gives a conditional median under lognormal errors; estimating an original-scale mean requires [bias correction after an inverse transformation](../../../../../../bias-correction-after-an-inverse-transformation.md). Also, the public archive's metadata describe some historical measures differently from the exam wording, so the fitted Donations effect is interpreted only on its recorded scale.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
