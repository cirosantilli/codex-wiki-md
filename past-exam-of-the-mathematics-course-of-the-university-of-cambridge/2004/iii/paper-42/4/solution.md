<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume a symmetric second-order [probability density function](../../../../../probability-density-function.md) [kernel for density estimation](../../../../../kernel-for-density-estimation.md) and enough smoothness for the displayed derivative functionals. The benchmark [smoothing bandwidth](../../../../../smoothing-bandwidth.md) is $h_0=[R(K)/(n\mu_2(K)^2R(f''))]^{1/5}$, balancing $R(K)/(nh)$ against $h^4\mu_2(K)^2R(f'')/4$. Three widely used selection methods are as follows.

For [least-squares density cross-validation](../../../../../least-squares-cross-validation-for-density-bandwidth.md), expand integrated squared error as $R(\widehat f_h)-2\int\widehat f_h f+R(f)$. Estimate the middle integral by leaving out the observation at which the estimate is evaluated, and minimize

$$
\operatorname{CV}(h)=R(\widehat f_h)-\frac2n\sum_i\widehat f_{h,-i}(X_i),\qquad\widehat f_{h,-i}(x)=\frac1{n-1}\sum_{j\ne i}K_h(x-X_j).
$$

The left-out observation is independent of its estimator, so the second term has expectation $-2\int(K_h*f)f$. Thus $\mathbb E\operatorname{CV}(h)=\operatorname{MISE}(h)-R(f)$ exactly. The subtraction of the self-contribution is essential. Computation uses $R(\widehat f_h)=n^{-2}\sum_{i,j}(K_h*\widetilde K_h)(X_i-X_j)$, where $\widetilde K_h(u)=K_h(-u)$. This method directly targets integrated error without estimating a curvature functional first. Under standard smoothness and a suitable search interval its selected [smoothing bandwidth](../../../../../smoothing-bandwidth.md) is ratio-consistent with the MISE optimum, and hence with $h_0$. Relative fluctuations are ordinarily $O_p(n^{-1/10})$, so the selected values can be quite variable in finite samples.

For [biased density cross-validation](../../../../../biased-cross-validation-for-density-bandwidth.md), estimate curvature from the second-derivative [probability density function](../../../../../probability-density-function.md) estimator and subtract its diagonal [variance](../../../../../variance-split.md) term:

$$
\widehat A_h=R(\widehat f_h'')-\frac{R(K'')}{nh^5},\qquad\operatorname{BCV}(h)=\frac{R(K)}{nh}+\frac{\mu_2(K)^2h^4}{4}\widehat A_h.
$$

Differentiating the [kernel for density estimation](../../../../../kernel-for-density-estimation.md) estimator and applying the integrated-variance identity gives the exact expectation $\mathbb ER(\widehat f_h'')=R(K'')/(nh^5)+(1-n^{-1})R(K_h*f'')$. Under the derivative regularity assumptions, $R(K_h*f'')=R(f'')+O(h^2)$, so $\mathbb E\widehat A_h=R(f'')+O(h^2)+O(n^{-1})$. Minimize BCV over a reasonable [smoothing bandwidth](../../../../../smoothing-bandwidth.md) range. It is a smoothed criterion directed at AMISE; the name reflects its finite-sample [bias](../../../../../bias-of-an-estimator.md) rather than an exact unbiased-risk identity. Standard conditions again give ratio consistency and relative fluctuation order $n^{-1/10}$. It often has a smoother objective than ordinary least-squares cross-validation, though numerical behavior and relative [variance](../../../../../variance-split.md) depend on the [probability density function](../../../../../probability-density-function.md) and [kernel for density estimation](../../../../../kernel-for-density-estimation.md).

For [plug-in bandwidth selection](../../../../../plug-in-bandwidth-selection.md), obtain an independent pilot scale g, estimate $A=R(f'')$, then set

$$
\boxed{\widehat h_{\rm PI}=\left[\frac{R(K)}{n\mu_2(K)^2\widehat A}\right]^{1/5}.}
$$

The pilot should be positive and stable; consistent positive estimates make this expression ratio-consistent by continuity. A simple normal-reference initialization uses $R(f'')=3/(8\sqrt\pi\,\sigma^5)$ under a normal reference model, substituting a sample scale for sigma. For a [Gaussian density kernel](../../../../../gaussian-density-kernel.md) this gives $h\approx1.06\widehat\sigma n^{-1/5}$. A pure normal-reference rule is quick but is asymptotically correctly calibrated only when its assumed curvature matches the actual [probability density function](../../../../../probability-density-function.md); it is useful as the first stage of a data-driven plug-in procedure.

A more adaptive [fourth-derivative pilot estimate of density curvature](../../../../../fourth-derivative-pilot-estimate-of-density-curvature.md) uses $R(f'')=\int ff^{(4)}$, obtained by two integrations by parts, and estimates it by

$$
\widehat R_g^{(2)}=\frac1n\sum_i\widehat f_g^{(4)}(X_i)=\frac1{n^2}\sum_{i,j}K_g^{(4)}(X_i-X_j).
$$

The diagonal expectation contributes $K^{(4)}(0)/(ng^5)$; the leading smoothing [bias](../../../../../bias-of-an-estimator.md) is $-g^2\mu_2(K)R(f''')/2$. Balancing these terms produces the stated pilot scale $g\asymp R(f''')^{-1/7}n^{-1/7}$, with another pilot or reference model supplying $R(f''')$. Under sufficient derivatives and tail control, its error is bounded by

$$
O_p\left(g^2+\frac1{ng^5}+n^{-1/2}+\frac1{ng^{9/2}}\right)=O_p(n^{-2/7})
$$

at that pilot scale. [Taylor expansion](../../../../../taylor-expansion.md) of the fifth-root formula gives $\widehat h_{\rm PI}/h_0-1=-(\widehat A-A)/(5A)+o_p(|\widehat A-A|)$, so it inherits that bound. A calibrated cancellation of leading pilot [bias](../../../../../bias-of-an-estimator.md) can give a faster rate. This illustrates why an appropriately constructed plug-in selector can converge more quickly than cross-validation, while requiring more smoothness and pilot choices. For each ratio-consistent method, its attained AMISE divided by the minimal AMISE tends to one.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
