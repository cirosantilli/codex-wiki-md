<h1 id="o/o5/solution">Solution</h1>

↑ **Parent:** [O5](../o5.md)

For a normal sample of size $m$,

$$
\bar X=\frac1m\sum_{i=1}^mX_i,\qquad S_X^2=\frac1{m-1}\sum_{i=1}^m(X_i-\bar X)^2.
$$

Then $\bar X\sim N(\mu_X,\sigma^2/m)$ and $cS_X^2\sim\chi^2_{m-1}$ with $c=(m-1)/\sigma^2$. These two statistics are independent.

Combining the difference distribution and pooled [variance](../../../../variance-split.md) calculation gives, with $\nu=m+n-2$,

$$
T_*=\frac{\bar X-\bar Y-(\mu_X-\mu_Y)}{S\sqrt{1/m+1/n}}\sim t_\nu.
$$

**The printed statistic has the sign of the centering term reversed.** Its numerator subtracts $\mu_Y-\mu_X$, so it is not generally a central Student statistic; the corrected centering above is necessary. Under the [null hypothesis](../../../../null-hypothesis.md) $\mu_X=\mu_Y$, the two expressions coincide, so the requested test is unaffected. Reject the two-sided null at significance level $\alpha$ when

$$
\left|\frac{\bar X-\bar Y}{S\sqrt{1/m+1/n}}\right|>t_{\nu,1-\alpha/2}.
$$

Here $\nu=8$ and $|T|=2.19<2.31$, so **do not reject at the 5% level**. This does not establish equality of the population means.

Age matching means that the two observations in a pair share an age effect, while ages vary across pairs. The independent, identically distributed two-sample model no longer represents this design: random pair effects induce within-pair dependence, and fixed differing ages can instead produce different individual means. Pairing by itself need not cause stochastic dependence when ages are treated as fixed. The appropriate alternative is a **[paired t-test](../../../../paired-t-test.md)** on the within-pair differences. Removing shared age [variation](../../../../variation.md) can reduce the noise and improve power when age strongly affects volume and the members of a pair are positively associated. Improvement is not automatic, since the paired test also uses fewer [degrees of freedom](../../../../degree-of-freedom.md).

## ↑ Ancestors (12)

1. [O5](../o5.md)
2. [O](../../o.md)
3. [2008 printed variant](../../../2008-printed-variant-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
