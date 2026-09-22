<h1 id="28j/solution">Solution</h1>

↑ **Parent:** [28J](../28j.md)

Put

$$
\overline X=\frac1n\sum_{i=1}^nX_i,
\qquad
S=\sum_{i=1}^n(X_i-\overline X)^2,
\qquad
\widehat\sigma^2=\frac Sn.
$$

The [log-likelihood](../../../../../log-likelihood.md), apart from an additive constant, is

$$
\ell_n(\mu,\sigma^2)
=-\frac n2\log\sigma^2
-\frac1{2\sigma^2}\sum_{i=1}^n(X_i-\mu)^2.
$$

Over the full parameter space its [maximum-likelihood estimates](../../../../../maximum-likelihood-estimation.md) are $(\widehat\mu,\widehat\sigma^2)=(\overline X,S/n)$. Under $H_0$, maximizing over the nuisance parameter $\mu$ gives $(\widehat\mu_0,\sigma_0^2)=(\overline X,1)$. Thus the generalized [likelihood-ratio test](../../../../../likelihood-ratio-test.md) statistic, in the convention $2(\sup_\Theta\ell_n-\sup_{\Theta_0}\ell_n)$, is

$$
\begin{aligned}
\Lambda_n(\Theta,\Theta_0)
&=2\{\ell_n(\overline X,S/n)-\ell_n(\overline X,1)\}\\
&=S-n-n\log(S/n)\\
&=n\{\widehat\sigma^2-1-\log\widehat\sigma^2\}.
\end{aligned}
$$

Under $H_0$, the normal-sample decomposition gives

$$
S\sim\chi^2_{n-1}.
$$

Writing $Z_n=(S-(n-1))/\sqrt{2(n-1)}$, the [central limit theorem](../../../../../central-limit-theorem.md) for a sum of squared independent standard normal variables yields $Z_n\xrightarrow dN(0,1)$. Hence [Slutsky theorem](../../../../../slutsky-theorem.md) gives

$$
\sqrt n(\widehat\sigma^2-1)
=\frac{S-n}{\sqrt n}
=\sqrt{\frac{2(n-1)}n}\,Z_n-\frac1{\sqrt n}
\xrightarrow dN(0,2),
$$

and in particular $\widehat\sigma^2\xrightarrow P1$.

For $h(x)=x-1-\log x$, [Taylor theorem](../../../../../taylor-theorem.md) at $x=1$ gives

$$
h(x)=\frac12(x-1)^2+o((x-1)^2).
$$

Consequently

$$
\Lambda_n
=\frac12\{\sqrt n(\widehat\sigma^2-1)\}^2+o_P(1)
\xrightarrow d Z^2,
\qquad Z\sim N(0,1),
$$

by the [continuous mapping theorem](../../../../../continuous-mapping-theorem.md) and Slutsky's theorem. Since the square of a standard normal variable has the [chi-squared distribution](../../../../../chi-squared-distribution.md) with one degree of freedom,

$$
\boxed{\Lambda_n(\Theta,\Theta_0)\xrightarrow d\chi_1^2.}
$$

## ↑ Ancestors (10)

1. [28J](../28j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
