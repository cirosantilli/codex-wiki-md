<h1 id="b/4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At maturity, one stock share is worth $(X_T-m)^+/n$. For a nonnegative strike $K$, the [digital call option](../../../../../digital-call-option.md) therefore pays one exactly on

$$
\frac{(X_T-m)^+}n>K\quad\Longleftrightarrow\quad X_T>m+nK.
$$

Under the [risk-neutral measure](../../../../../risk-neutral-measure.md), $\log(X_T/x_0)$ is normal with mean $(r-\sigma^2/2)T$ and variance $\sigma^2T$. The [risk-neutral pricing](../../../../../risk-neutral-pricing.md) consequently gives

$$
\boxed{V_0=e^{-rT}\Phi\left(\frac{\log(x_0/(m+nK))+(r-\sigma^2/2)T}{\sigma\sqrt T}\right).}
$$

The effective company-value strike is $m+nK$, because both the outstanding debt and the number of shares matter. At $K=0$, the strict positive-share event remains $X_T>m$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
