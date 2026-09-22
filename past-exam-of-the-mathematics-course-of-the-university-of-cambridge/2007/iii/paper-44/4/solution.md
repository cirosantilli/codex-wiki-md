<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume $n\geq2$, so the residual sum of squares is positive almost surely. Write $\overline Y=n^{-1}\sum_iY_i$ and $S=\sum_i(Y_i-\overline Y)^2$. The [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell(\mu,\sigma^2)=-\frac n2\log(2\pi\sigma^2)-\frac1{2\sigma^2}\sum_i(Y_i-\mu)^2.
$$

The decomposition $\sum_i(Y_i-\mu)^2=S+n(\overline Y-\mu)^2$ shows that, at every fixed positive variance, its constrained [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) of the mean is $\overline Y$. Substituting this mean and differentiating with respect to the variance gives

$$
\boxed{\widehat\mu_{\sigma^2}=\overline Y,\qquad\widehat\sigma^2=\frac Sn.}
$$

The denominator $n$ is required by [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md); $S/(n-1)$ is the unbiased variance estimate, which is a different estimator.

Under the null variance $\sigma_0^2$, maximize over the same mean $\overline Y$. Subtracting the null maximum [log-likelihood](../../../../../log-likelihood.md) from the unrestricted maximum gives the [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md)

$$
W=2\{\ell(\overline Y,S/n)-\ell(\overline Y,\sigma_0^2)\}=n\log\frac{n\sigma_0^2}{S}+\frac S{\sigma_0^2}-n.
$$

By [Cochran's theorem](../../../../../cochran-s-theorem.md), the [residual sum of squares in a normal sample](../../../../../residual-sum-of-squares-in-a-normal-sample.md) satisfies $U=S/\sigma_0^2\sim\chi_{n-1}^2$ under the null. Set $V=(U-n)/n$, so $U/n=1+V>0$. Then

$$
\boxed{W=n\{-\log(1+V)+V\},\qquad U\sim\chi_{n-1}^2.}
$$

The normal mean is a [nuisance parameter](../../../../../nuisance-parameter.md), but this null law does not depend on it.

A [Bartlett correction](../../../../../bartlett-correction.md) removes the first-order discrepancy between the null mean of a regular [likelihood-ratio test statistic](../../../../../likelihood-ratio-test-statistic.md) and the degrees of freedom of its limiting [chi-squared distribution](../../../../../chi-squared-distribution.md). In the convention used here, if the limiting degrees of freedom are $d$ and

$$
\mathbb E_0W=d\left(1+\frac bn+O(n^{-2})\right),
$$

then $b$ is the [Bartlett correction coefficient](../../../../../bartlett-correction-coefficient.md), also called the [Bartlett correction factor](../../../../../bartlett-correction-coefficient.md), and the [Bartlett-corrected likelihood-ratio statistic](../../../../../bartlett-corrected-likelihood-ratio-statistic.md) is $W_B=W/(1+b/n)$. Its null mean is $d+O(n^{-2})$. The finite-$n$ divisor is $1+b/n$, rather than $b$ itself. There is one restriction on the variance here, so $d=1$.

Expand the logarithm around $V=0$ and use the permitted termwise asymptotic integration:

$$
\mathbb E_0W=n\left\{\frac{\mathbb EV^2}{2}-\frac{\mathbb EV^3}{3}+\frac{\mathbb EV^4}{4}-\frac{\mathbb EV^5}{5}+\cdots\right\}.
$$

Using the supplied raw moments of the [chi-squared distribution](../../../../../chi-squared-distribution.md) and expanding $(U-n)^r$ gives

$$
\mathbb EV^2=\frac{2n-1}{n^2},\qquad\mathbb EV^3=\frac{2n-3}{n^3},\qquad\mathbb EV^4=\frac{12n^2+4n-15}{n^4}.
$$

For instance, $\mathbb EU=n-1$ and $\mathbb EU^2=(n-1)(n+1)$ give the first formula after subtracting $2n\mathbb EU-n^2$. The same binomial expansion, using the raw third and fourth moments, gives the other two formulas.

We must justify why higher moments cannot change the $n^{-1}$ coefficient. Represent $U=\sum_{i=1}^{n-1}Z_i^2$ for independent standard normal variables, and put $T_i=Z_i^2-1$. Each $T_i$ is centered and has all absolute moments finite. With $H=\sum_{i=1}^{n-1}T_i$, one has $V=(H-1)/n$. The supplied centered-sum bounds say, for each fixed integer $j\geq2$,

$$
|\mathbb EH^j|=\begin{cases}O(n^{j/2})&j\text{ even},\\O(n^{(j-1)/2})&j\text{ odd}.\end{cases}
$$

Also $\mathbb EH=0$ and $\mathbb EH^0=1$. Therefore, for every fixed $r\geq2$, expanding $(H-1)^r$ gives

$$
|\mathbb EV^r|\leq n^{-r}\sum_{j=0}^r\binom rj|\mathbb EH^j|=O\big(n^{-\lceil r/2\rceil}\big).
$$

These are bounds on the absolute values of signed moments; the odd-moment estimate must not be misread as a bound on $\mathbb E|H|^j$. In particular, each fixed Taylor term of degree $r\geq5$ has $n\mathbb EV^r=O(n^{-2})$ or smaller. Combined with the question's permission to integrate the asymptotic expansion term by term, this controls the higher-order contribution at the required order. It does not require a globally convergent Taylor series for every realized $V$.

Substituting the first three moment formulas now gives

$$
\begin{aligned}
\mathbb E_0W&=\left(1-\frac1{2n}\right)-\left(\frac2{3n}+O(n^{-2})\right)+\left(\frac3n+O(n^{-2})\right)+O(n^{-2})\\
&=1+\frac1n\left(-\frac12-\frac23+3\right)+O(n^{-2})\\
&=1+\frac{11}{6n}+O(n^{-2}).
\end{aligned}
$$

Thus the [Bartlett correction for a normal variance with unknown mean](../../../../../bartlett-correction-for-a-normal-variance-with-unknown-mean.md) is

$$
\boxed{b=\frac{11}{6},\qquad W_B=\frac{W}{1+11/(6n)}.}
$$

Its null mean is $1+O(n^{-2})$, and the usual reference law is $\chi_1^2$. Keeping the estimated mean's loss of one residual degree of freedom, and using the maximum-likelihood variance divisor $n$, are both essential to the coefficient $11/6$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
