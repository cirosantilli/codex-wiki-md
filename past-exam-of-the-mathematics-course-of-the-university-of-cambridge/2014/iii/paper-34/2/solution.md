<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) sampled from a [probability density function](../../../../../probability-density-function.md) $f$, a [kernel density estimator](../../../../../kernel-density-estimation.md) with [kernel for density estimation](../../../../../kernel-for-density-estimation.md) $K$ and [smoothing bandwidth](../../../../../smoothing-bandwidth.md) $h>0$ is

$$
\widehat f_h(x)=\frac1n\sum_{i=1}^n K_h(x-X_i),\qquad K_h(u)=h^{-1}K(u/h),\qquad \int K=1.
$$

The usual [kernel for density estimation](../../../../../kernel-for-density-estimation.md) is nonnegative; finite $\int K^2$ makes the integrated [variance](../../../../../variance-split.md) finite. The [mean integrated squared error](../../../../../integrated-mean-squared-error.md) and its [bias-variance decomposition of mean squared error](../../../../../bias-variance-decomposition-of-mean-squared-error.md) are

$$
\operatorname{MISE}(\widehat f_h)=\mathbb E\int_{\mathbb R}(\widehat f_h(x)-f(x))^2\,dx
=\int\operatorname{Bias}(\widehat f_h(x))^2\,dx+\int\operatorname{Var}(\widehat f_h(x))\,dx.
$$

The interchange is justified by the [Tonelli theorem](../../../../../tonelli-theorem.md).

For the [exponential distribution](../../../../../exponential-distribution.md) and the specified unit-width [uniform kernel](../../../../../uniform-smoothing-kernel.md), put $g_h(x)=\mathbb E\widehat f_h(x)$. The [expected value](../../../../../expected-value.md) is $h^{-1}\mathbb P\{x-h/2\leq X\leq x+h/2\}$. Intersecting this interval with the positive half-line gives

$$
\boxed{g_h(x)=\frac{e^{-\max(x-h/2,0)}-e^{-\max(x+h/2,0)}}h.}
$$

On $[-h/4,0)$ the true [probability density function](../../../../../probability-density-function.md) vanishes, whereas

$$
g_h(x)=\frac{1-e^{-(x+h/2)}}h\geq\frac{1-e^{-h/4}}h\geq\frac18\qquad(0<h\leq1).
$$

Here $1-e^{-z}\geq z/2$ for $0\leq z\leq1/4$. This leakage across the support boundary proves the [integrated squared bias from a density jump](../../../../../integrated-squared-bias-from-a-density-jump.md):

$$
\boxed{B(h):=\int(g_h-f)^2\,dx\geq h/256\qquad(0<h\leq1).}
$$

In particular, $h_0=1$ and $c=1/256$ suffice. The phenomenon differs from a smooth interior [bias of a kernel density estimator](../../../../../bias-of-a-kernel-density-estimator.md): the order-one boundary error persists over a region of width proportional to $h$.

By [independence](../../../../../independent-random-variables.md), $\operatorname{Var}(\widehat f_h(x))=n^{-1}\{\mathbb E K_h(x-X)^2-g_h(x)^2\}$. Integrating the first term and using $\int K^2=1$ yields

$$
\boxed{\int\operatorname{Var}(\widehat f_h(x))\,dx=\frac1{nh}-\frac{I(h)}n,\qquad I(h)=\int g_h(x)^2\,dx.}
$$

Also $I(h)\leq\int f^2=1/2$: the [kernel density estimator](../../../../../kernel-density-estimation.md) mean is an average of translates of $f$, so the [Jensen inequality](../../../../../jensen-s-inequality.md) followed by the [Tonelli theorem](../../../../../tonelli-theorem.md) bounds its squared integral.

To optimize over every $h>0$, we must establish that useful [smoothing bandwidths](../../../../../smoothing-bandwidth.md) approach zero, rather than optimize only a formal small-$h$ expression. An exact calculation supplies that justification. The autocorrelation integral of the [exponential distribution](../../../../../exponential-distribution.md) density is

$$
\int f(x-u)f(x-v)\,dx=\tfrac12e^{-|u-v|}.
$$

Averaging over the two uniform windows, or integrating the piecewise expression for $g_h$, gives

$$
I(h)=\frac{h-1+e^{-h}}{h^2},\qquad
\int f g_h=\frac{1-e^{-h/2}}h,
\qquad B(h)=\frac12+\frac{h-1+e^{-h}}{h^2}-\frac{2(1-e^{-h/2})}h.
$$

These formulas show that $B$ is continuous on $(0,\infty)$, is strictly positive there because $g_h>0$ on $(-h/2,0)$, and tends to $1/2$ as $h\to\infty$. Consequently, $B$ is bounded away from zero on $[\delta,\infty)$ for every $\delta>0$. Its expansion agrees with the supplied $B(h)=h/12+o(h)$.

The choice $h_n=\sqrt{12/n}$ gives

$$
\sqrt n\operatorname{MISE}(\widehat f_{h_n})\longrightarrow\frac1{\sqrt3}.
$$

Choose [smoothing bandwidths](../../../../../smoothing-bandwidth.md) within $1/n$ of the [infimum](../../../../../infimum.md). Their [mean integrated squared error](../../../../../integrated-mean-squared-error.md) tends to zero, and nonnegativity of the integrated [variance](../../../../../variance-split.md) gives $B(h_n)\to0$, hence $h_n\to0$. For any $\varepsilon\in(0,1/12)$, eventually

$$
\operatorname{MISE}(\widehat f_{h_n})
\geq(1/12-\varepsilon)h_n+\frac1{nh_n}-\frac1{2n}
\geq2\sqrt{\frac{1/12-\varepsilon}{n}}-\frac1{2n}.
$$

The last step is the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md). Taking the lower limit and then $\varepsilon\downarrow0$ matches the upper bound. Thus

$$
\boxed{\sqrt n\inf_{h>0}\operatorname{MISE}(\widehat f_h)\longrightarrow\frac1{\sqrt3}.}
$$

The original PDF has this constant; the TeX aid's $1/\sqrt2$ is a transcription error.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 34](../../paper-34-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
