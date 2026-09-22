<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $p=\Phi(1)-\Phi(0)$, and write $\varphi$ for the [standard normal distribution](../../../../../../standard-normal-distribution.md) density. For [importance sampling](../../../../../../importance-sampling.md), choose the proposal density $q(x)=\mathbf1_{[0,1]}(x)$, namely the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on the target interval. Its [importance sampling](../../../../../../importance-sampling.md) weight is

$$
\boxed{w(x)=\frac{f(x)}{q(x)}=\frac{\varphi(x)}p\quad(0\leq x\leq1).}
$$

For iid uniform draws $U_1,\ldots,U_N$,

$$
\boxed{\widehat\mu_{\mathrm{IS}}=\frac1N\sum_{i=1}^N\frac{U_i\varphi(U_i)}p}
$$

is an [unbiased estimator](../../../../../../unbiased-estimator.md) of the target mean, since its expectation integrates $xf(x)$. If one chooses not to evaluate $p$, the [self-normalized importance sampling](../../../../../../self-normalized-importance-sampling.md) alternative $\sum U_i\varphi(U_i)/\sum\varphi(U_i)$ has [statistical consistency](../../../../../../consistency-statistics.md), but generally is not an [unbiased estimator](../../../../../../unbiased-estimator.md).

Alternatively, draw [independent random variables](../../../../../../independent-random-variables.md) $V_1,\ldots,V_N$ with the [standard normal distribution](../../../../../../standard-normal-distribution.md), let $A_i=\mathbf1_{\{0\leq V_i\leq1\}}$ and $K=\sum A_i$, and use

$$
\boxed{\widehat\mu_{\mathrm{keep}}=\frac{\sum_iA_iV_i}{K}\quad(K>0).}
$$

Conditionally on $K=k>0$, the retained draws are iid from the [truncated normal distribution](../../../../../../truncated-normal-distribution.md), so their average is an [unbiased estimator](../../../../../../unbiased-estimator.md) with [variance](../../../../../../variance-split.md) $\tau^2/k$, where $\tau^2$ is its [variance](../../../../../../variance-split.md). If $K=0$ the ratio is undefined; one can continue drawing until a prescribed number of retained observations is obtained.

Here [importance sampling](../../../../../../importance-sampling.md) uses every draw inside the interval, whereas only $p\approx0.3413$ of the normal proposals are retained. The advantage can also be quantified. Integration using $\varphi'(x)=-x\varphi(x)$ gives

$$
\mu=\frac{\varphi(0)-\varphi(1)}p\approx0.459862,
\qquad\tau^2=1-\frac{\varphi(1)}p-\mu^2\approx0.079652.
$$

For uniform [importance sampling](../../../../../../importance-sampling.md),

$$
N\operatorname{Var}(\widehat\mu_{\mathrm{IS}})=\frac1{p^2}\int_0^1x^2\varphi(x)^2\,dx-\mu^2\approx0.047336.
$$

For the retained-draw ratio with a fixed total proposal budget, its [asymptotic variance](../../../../../../asymptotic-variance.md) coefficient is $\tau^2/p\approx0.233347$. Thus this importance choice has substantially smaller error for the same proposal count; it also avoids wasting about two thirds of the [standard normal distribution](../../../../../../standard-normal-distribution.md) draws. This comparison is specific to this well-matched [importance sampling](../../../../../../importance-sampling.md) proposal; arbitrary proposal choices do not share this guarantee.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
