<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There is a genuine normalization error in the printed function. Write $Y_i\sim\operatorname{Unif}(0,2)$ independently, $g(y)=1/(\pi(1+y^2))$ and $H(y)=y^2-4/3$. The internal sum produces a scalar; taking its mean does not divide by $n$. The literal returned value is therefore

$$
T_{\beta,\mathrm{printed}}=\frac12-2\sum_{i=1}^n\{g(Y_i)-\beta H(Y_i)\}.
$$

Since $\mathbb EH=0$ and $\mathbb Eg=\arctan(2)/(2\pi)=1/4-\theta/2$, its expectation is

$$
\mathbb E T_{\beta,\mathrm{printed}}=n\theta+\frac{1-n}{2}.
$$

It does not estimate $\theta$ unbiasedly unless $n=1$, and no fixed [control variate](../../../../../../control-variates.md) coefficient removes this bias. In particular the actual call with $\beta=0$ returns

$$
\boxed{\check\theta_{\mathrm{printed}}=\frac12-2\sum_{i=1}^n\frac1{\pi(1+Y_i^2)}.}
$$

This is an instance of [summing before taking a mean changes Monte Carlo normalization](../../../../../../summing-before-taking-a-mean-changes-monte-carlo-normalization.md).

The intended corrected method replaces the sum by a [sample mean](../../../../../../sample-mean.md):

$$
T_\beta=\frac12-\frac2n\sum_{i=1}^n\{g(Y_i)-\beta H(Y_i)\}.
$$

It uses symmetry to write the tail as $\theta=1/2-\int_0^2g(y)\,dy$, then [Monte Carlo integration](../../../../../../monte-carlo-integration.md) on a bounded interval, and finally a mean-zero [control variate](../../../../../../control-variates.md). For $\beta=0$ the intended estimator is $1/2-(2/n)\sum_i g(Y_i)$, whose summands are smooth and bounded. Keeping the average normalization, $\mathbb ET_\beta=\theta$ and

$$
\operatorname{Var}(T_\beta)=\frac4n\{\operatorname{Var}(g)-2\beta\operatorname{Cov}(g,H)+\beta^2\operatorname{Var}(H)\}.
$$

Differentiating this quadratic gives the [Cauchy tail control variate on a bounded interval](../../../../../../cauchy-tail-control-variate-on-a-bounded-interval.md) coefficient

$$
\beta_* =\frac{\operatorname{Cov}(g,H)}{\operatorname{Var}(H)}.
$$

Here $\mathbb EY^2=4/3$, $\mathbb EY^4=16/5$, so $\operatorname{Var}(H)=64/45$. Also

$$
\operatorname{Cov}(g,H)=\frac1{2\pi}\int_0^2\frac{y^2-4/3}{1+y^2}\,dy=\frac1\pi-\frac{7\arctan2}{6\pi}=\frac1\pi-\frac7{12}+\frac{7\theta}{6}.
$$

Consequently

$$
\boxed{\beta_* =\frac{45}{64}\left(\frac1\pi-\frac7{12}+\frac{7\theta}{6}\right)\approx-0.06528.}
$$

The negative sign is consistent with $g$ decreasing and $H$ increasing. One may estimate the [covariance](../../../../../../covariance.md) and [variance](../../../../../../variance-split.md) using a separate pilot sample and fix the resulting coefficient for a fresh sample. This coefficient minimizes the literal function's [variance](../../../../../../variance-split.md) as well, but its missing factor of $1/n$ still leaves the bias above.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
