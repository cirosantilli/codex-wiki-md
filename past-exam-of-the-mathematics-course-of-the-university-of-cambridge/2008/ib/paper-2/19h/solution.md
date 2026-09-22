<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

Write $r=1-\alpha-\beta>0$. Differentiating the [probability generating function](../../../../../probability-generating-function.md) at $(1,1)$ gives

$$
\boxed{\mathbb E[X]=\frac\alpha r},\qquad \mathbb E[Y]=\frac\beta r.
$$

Expanding its denominator as a [geometric series](../../../../../geometric-series.md) and then applying the [binomial theorem](../../../../../binomial-theorem.md) gives

$$
\frac r{1-\alpha s-\beta t}
=r\sum_{k\ge0}(\alpha s+\beta t)^k
=r\sum_{x,y\ge0}\binom{x+y}{x}\alpha^x\beta^y s^xt^y.
$$

Coefficient identification proves $\boxed{\Pr(X=x,Y=y)=r\binom{x+y}{x}\alpha^x\beta^y}$, a one-stop [negative multinomial distribution](../../../../../negative-multinomial-distribution.md).

For an independent identically distributed sample let $S_X=\sum X_i$ and $S_Y=\sum Y_i$. Ignoring parameter-independent factors, the log-likelihood is $\ell=n\ln r+S_X\ln\alpha+S_Y\ln\beta$. When both sums are positive, its stationary equations are $S_X/\alpha=n/r$ and $S_Y/\beta=n/r$. Together with $r+\alpha+\beta=1$, these give

$$
\boxed{\widehat\alpha=\frac{S_X}{n+S_X+S_Y}
=\frac{\overline X}{1+\overline X+\overline Y},\qquad
\widehat\beta=\frac{S_Y}{n+S_X+S_Y}.}
$$

The Hessian is $-(n/r^2)\mathbf1\mathbf1^T-\operatorname{diag}(S_X/\alpha^2,S_Y/\beta^2)$, negative definite in this case, so the stationary point is the unique global maximum.

There is an important boundary qualification: if $S_X=0$, the derivative with respect to $\alpha$ is $-n/r<0$, so the likelihood increases as $\alpha$ decreases to zero. The displayed formula then gives a boundary estimator, not an attained MLE in the stated open parameter space $\alpha,\beta>0$. The analogous issue holds for $S_Y=0$. The formulas are MLEs on the extension allowing zero category probabilities, and interior MLEs when both counts are positive.

For bias, put $p=\alpha+\beta$ and $U=(S_X+S_Y)/n$. Then $\mathbb E[U]=p/(1-p)$ and $\widehat\alpha+\widehat\beta=g(U)$ with $g(u)=u/(1+u)$. Its second derivative is $-2/(1+u)^3<0$, and $U$ is nondegenerate. Strict [Jensen's inequality](../../../../../jensen-s-inequality.md) gives

$$
\mathbb E[\widehat\alpha+\widehat\beta]<g(\mathbb E U)=p.
$$

In fact both estimates are downward biased. Conditional on $X_i+Y_i$, the first count is binomial with success probability $\alpha/p$; hence conditional on $S=S_X+S_Y$, $S_X$ is also binomial with that probability. Therefore

$$
\mathbb E[\widehat\alpha]=\frac\alpha p\mathbb E\left[\frac S{n+S}\right]<\alpha,
\qquad \mathbb E[\widehat\beta]<\beta.
$$

This proves the [finite-sample bias in a negative multinomial probability estimator](../../../../../finite-sample-bias-in-a-negative-multinomial-probability-estimator.md), using the boundary-extended formulas whenever necessary.

Finally, the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) applies because the nonnegative variables have finite means: almost surely $\overline X\to\alpha/r$ and $\overline Y\to\beta/r$. [Continuity](../../../../../continuous-function.md) of the estimator function then gives

$$
\boxed{\widehat\alpha\longrightarrow\frac{\alpha/r}{1+\alpha/r+\beta/r}=\alpha\quad\text{almost surely},}
$$

and similarly for $\widehat\beta$. Thus the estimates are strongly consistent despite finite-sample bias. Almost surely both sample sums eventually become positive, so the open-parameter MLE issue affects finite samples rather than this asymptotic conclusion.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
