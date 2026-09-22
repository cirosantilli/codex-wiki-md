<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [grouped-binomial logistic regression](../../../../../../grouped-binomial-logistic-regression.md), $S_i\sim\operatorname{Bin}(C_i,p_i)$ and $\operatorname{logit}(p_i)=\eta_i$. Center the year as $u_i=i-7.5$. Maximizing $\ell=\sum_i[S_i\eta_i-C_i\ln(1+e^{\eta_i})]$ gives score $X^T(S-Cp)=0$ and information $X^T\operatorname{diag}\{C_ip_i(1-p_i)\}X$; these determine the estimates and working [covariance matrix](../../../../../../covariance-matrix.md).

A straight-line logit fit is $\widehat\eta=-1.95965+0.045384u$, with naive binomial standard errors $0.005382$ and $0.001352$. Its yearly odds multiplier is $e^{0.045384}=1.04643$, with naive 95% [Wald confidence interval](../../../../../../wald-confidence-interval.md) $[1.04366,1.04921]$. However, its residual [deviance](../../../../../../exponential-family-deviance.md) is $58.20$ on 12 degrees of freedom ($p=4.8\times10^{-8}$), so those small standard errors do not describe an adequate independent-binomial fit.

Comparing polynomial mean structures gives residual deviances $1191.73,58.20,55.70,27.08$ for degrees zero through three, with respective residual degrees of freedom $13,12,11,10$. A quadratic term alone adds little; the cubic structure captures the middle-period acceleration and later leveling. Even the cubic independent-binomial fit has $p=0.00253$ for its residual [deviance goodness-of-fit test](../../../../../../deviance-goodness-of-fit-test.md). A useful working model is therefore cubic [quasibinomial regression](../../../../../../quasibinomial-regression.md), retaining the logistic mean and estimating [overdispersion](../../../../../../overdispersion.md) rather than claiming an exact binomial law:

$$
\boxed{\widehat\eta(u)=-1.953614+0.062138u-0.0002830u^2-0.0005812u^3.}
$$

The Pearson estimate is $\widehat\phi=27.182/10=2.718$. Using standard errors multiplied by $\sqrt{\widehat\phi}$ and a $t_{10}$ reference, the approximate 95% coefficient intervals are $[-1.98294,-1.92429]$, $[0.04982,0.07445]$, $[-0.001697,0.001131]$, and $[-0.000980,-0.000182]$. An approximate quasi-deviance comparison of cubic against linear gives $F_{2,10}=5.72$ and $p=0.022$, supporting the added shape while acknowledging that only fourteen annual groups inform dispersion.

In this preferred mean model the odds change is not constant:

$$
\boxed{\frac{\mathrm{odds}(i+1)}{\mathrm{odds}(i)}
=\exp\{\beta_1+\beta_2(2u+1)+\beta_3(3u^2+3u+1)\}.}
$$

The fitted annual change is larger around the middle than at the ends; the straight-line 4.6% increase is a useful overall summary, not an exact yearly effect in the cubic model. The fitted curve, uncertainty band and residual plot appear in the figure. **Singleton success increased overall, but a constant log-odds trend with unit binomial dispersion fits poorly.** Quasibinomial intervals remain working-model intervals: serial dependence, changing patient mix and treatment practices cannot be separated from annual aggregates alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
