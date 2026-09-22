<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a normalized [kernel for density estimation](../../../../../kernel-for-density-estimation.md) $K$, with $\int K=1$, the [kernel density estimator](../../../../../kernel-density-estimation.md) is

$$
\boxed{\widehat f_{n,h}(x)=\frac1{nh}\sum_{i=1}^nK\!\left(\frac{x-X_i}{h}\right).}
$$

It replaces each atom of the [empirical measure](../../../../../empirical-measure.md) by a translated, scaled copy of $K$: averaging these small probability-density bumps gives a smooth approximation to the sampling density. Integral one is part of the probability-kernel convention; without it, the estimator generally targets $f(x)\int K$.

**The printed bandwidth assumption is insufficient for the claimed normal limit.** The additional condition $nh_n\to\infty$ is needed at points with positive density. For a counterexample, take a [normal distribution](../../../../../normal-distribution.md) density $f$, $x=0$, the [unit-width box kernel](../../../../../unit-width-box-kernel.md) and $h_n=n^{-2}$. Then $nh_n^3\to0$, but the probability that any observation lies in the window is at most $n\|f\|_\infty h_n\to0$. On the complementary event the estimator is zero, and $\sqrt{nh_n}(\widehat f_{n,h_n}(0)-f(0))=-f(0)/\sqrt n\to0$. The limit in probability is therefore zero, whereas the stated normal limit has positive variance.

We now prove the intended [pointwise central limit theorem for a kernel density estimator](../../../../../pointwise-central-limit-theorem-for-a-kernel-density-estimator.md) under $h=h_n\to0$, $nh\to\infty$ and $nh^3\to0$. The first condition also follows from the last one. A [mean value theorem](../../../../../mean-value-theorem.md) bound, with $L=\|f'\|_\infty$, gives the [bias of a kernel density estimator](../../../../../bias-of-a-kernel-density-estimator.md)

$$
|\mathbb E\widehat f_{n,h}(x)-f(x)|
=\left|\int K(u)(f(x-hu)-f(x))\,du\right|
\le Lh\int|u|K(u)\,du.
$$

Thus the bias multiplied by $\sqrt{nh}$ tends to zero.

The [Lindeberg-Feller central limit theorem](../../../../../lindeberg-feller-central-limit-theorem.md) says that independent centered variables in each row of a triangular array have sum converging in distribution to $N(0,\sigma^2)$ if the sum of their variances tends to $\sigma^2>0$ and, for every $\eta>0$, the sum of their truncated second moments $\mathbb E[Z_{n,i}^2\mathbf1_{\{|Z_{n,i}|>\eta\}}]$ tends to zero. Put $Y_{n,i}=K((x-X_i)/h)$ and $Z_{n,i}=(Y_{n,i}-\mathbb EY_{n,i})/\sqrt{nh}$. The [independence](../../../../../independent-random-variables.md) hypothesis holds within each row. A change of variable gives

$$
\sum_{i=1}^n\operatorname{Var}(Z_{n,i})
=\frac{\operatorname{Var}(Y_{n,1})}{h}
=\int K(u)^2f(x-hu)\,du-h\left(\int K(u)f(x-hu)\,du\right)^2
\longrightarrow f(x)\|K\|_2^2.
$$

Continuity of $f$ at $x$ and the compact support and boundedness of $K$ justify the limit. Also $|Z_{n,i}|\le2\|K\|_\infty/\sqrt{nh}\to0$, so the [Lindeberg condition](../../../../../lindeberg-condition.md) is eventually identically zero for every $\eta$. The sum is exactly $\sqrt{nh}(\widehat f_{n,h}(x)-\mathbb E\widehat f_{n,h}(x))$. Combining the centered limit with the negligible bias by the [Slutsky theorem](../../../../../slutsky-theorem.md) proves

$$
\boxed{\sqrt{nh_n}(\widehat f_{n,h_n}(x)-f(x))\xrightarrow{d}N(0,f(x)\|K\|_2^2).}
$$

If $f(x)=0$, the centered variance tends to zero, and the [Chebyshev inequality](../../../../../chebyshev-inequality.md) proves the corresponding degenerate limit directly.

For $f(x)>0$, let $q_\beta$ be the supplied $\beta$-quantile of this limiting [normal distribution](../../../../../normal-distribution.md). Inverting the limiting central probability gives the [confidence interval](../../../../../confidence-interval.md)

$$
\boxed{\left[\widehat f_{n,h_n}(x)-\frac{q_{1-\alpha/2}}{\sqrt{nh_n}},\quad
\widehat f_{n,h_n}(x)-\frac{q_{\alpha/2}}{\sqrt{nh_n}}\right].}
$$

Continuity of the limiting distribution gives asymptotic coverage $1-\alpha$. Equivalently, its half-width is $z_{1-\alpha/2}\sqrt{f(x)\|K\|_2^2/(nh_n)}$ under the stipulated oracle quantiles. A degenerate limit at $f(x)=0$ does not by itself justify this nominal-coverage normal interval.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
