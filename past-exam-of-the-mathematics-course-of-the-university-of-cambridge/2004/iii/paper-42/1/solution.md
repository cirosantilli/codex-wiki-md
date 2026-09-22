<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [kernel for density estimation](../../../../../kernel-for-density-estimation.md) is an integrable function K of unit integral, ordinarily nonnegative and centered. Square integrability is needed for integrated [variance](../../../../../variance-split.md); a symmetric second-order [kernel for density estimation](../../../../../kernel-for-density-estimation.md) also has $\int uK(u)du=0$ and finite nonzero second moment $\mu_2(K)$. Its scaled form is $K_h(u)=h^{-1}K(u/h)$, and the [kernel density estimator](../../../../../kernel-density-estimation.md) is

$$
\widehat f_h(x)=\frac1n\sum_{i=1}^nK_h(x-X_i).
$$

Higher-order signed kernels are possible, but need not give a nonnegative [probability density function](../../../../../probability-density-function.md) estimate.

The [mean integrated squared error](../../../../../integrated-mean-squared-error.md) is $\mathbb E\int(\widehat f_h(x)-f(x))^2dx$. Put $g_h=K_h*f$. [Independence](../../../../../independent-random-variables.md) gives the pointwise [mean](../../../../../expected-value.md) $g_h$ and [variance](../../../../../variance-split.md) $n^{-1}[(K_h^2*f)-g_h^2]$. Integrating, use $\int f=1$ and Fubini to obtain $\int(K_h^2*f)=R(K_h)$. The bias-variance decomposition proves the exact formula

$$
\boxed{\operatorname{MISE}(\widehat f_h)=R(K_h*f-f)+\frac1n\{R(K_h)-R(K_h*f)\}.}
$$

Equivalently this is $R(f)-2\int f(K_h*f)+(1-n^{-1})R(K_h*f)+R(K)/(nh)$. These identities assume the displayed integrals are finite; they are exact, rather than a small-[smoothing bandwidth](../../../../../smoothing-bandwidth.md) expansion.

For a symmetric second-order [kernel for density estimation](../../../../../kernel-for-density-estimation.md), [Taylor expansion](../../../../../taylor-expansion.md) gives leading [bias](../../../../../bias-of-an-estimator.md) $h^2\mu_2(K)f''/2$, and the leading integrated [variance](../../../../../variance-split.md) is $R(K)/(nh)$. Thus the [asymptotic mean integrated squared error](../../../../../asymptotic-mean-integrated-squared-error.md) balances inverse [smoothing bandwidth](../../../../../smoothing-bandwidth.md) against fourth-power [bias](../../../../../bias-of-an-estimator.md), with optimal [smoothing bandwidth](../../../../../smoothing-bandwidth.md) $[R(K)/(n\mu_2(K)^2R(f''))]^{1/5}$. Its appearance of the [integrated squared density curvature](../../../../../integrated-squared-density-curvature.md) motivates the scale comparison.

For $f_a(x)=af(ax)$, $a>0$, two differentiations give $f_a''(x)=a^3f''(ax)$. A change of variables therefore gives $R(f_a'')=a^5R(f'')$, which tends to zero as $a\downarrow0$ if the original curvature integral is finite. The distribution with [probability density function](../../../../../probability-density-function.md) $f_a$ is that of X divided by a, so $\sigma(f_a)=\sigma(f)/a$. Consequently

$$
\boxed{D(f_a)=\sigma(f_a)^5R(f_a'')=\sigma(f)^5R(f'')=D(f).}
$$

This [scale-invariant density curvature](../../../../../scale-invariant-density-curvature.md) measures shape without dependence on the units used to measure X.

For the final minimization, write $c=35/32$ and use the [triweight kernel](../../../../../triweight-kernel.md) $f_0=c(1-x^2)^3$ on $(-1,1)$, zero outside. Integration gives total mass one, [mean](../../../../../expected-value.md) zero and [variance](../../../../../variance-split.md) $1/9$. Its value and its first two derivatives vanish at both endpoints, so its extension is twice continuously differentiable. On the interior,

$$
f_0''=c(-6+36x^2-30x^4),\qquad f_0'''=c(72x-120x^3),\qquad f_0^{(4)}=c(72-360x^2).
$$

In particular $f_0'''(1)=-48c$ and $f_0'''(-1)=48c$.

Put $e=h-f_0$. The mass and moment constraints give $\int e=\int x^2e=0$, since both means vanish and their variances match. If $R(h'')=\infty$ the claim is immediate; otherwise expand the squared norm and integrate its cross term twice by parts over $[-1,1]$. The first endpoint term vanishes because $f_0''(\pm1)=0$, but the next one must be retained:

$$
\begin{aligned}
\int e''f_0''&=-[ef_0''']_{-1}^1+c\int_{-1}^1(72-360x^2)e(x)dx\\
&=48c\{h(1)+h(-1)\}+c\int_{|x|>1}(360x^2-72)h(x)dx\geq0.
\end{aligned}
$$

For the second equality use the zero mass and second moment of e and $e=h\geq0$ outside the support. All terms in the last expression are nonnegative, including the endpoint values of a [probability density function](../../../../../probability-density-function.md). It follows that

$$
\boxed{R(h'')=R(f_0'')+R(e'')+2\int e''f_0''\geq R(f_0'')=35.}
$$

This proves that the [triweight density minimizes integrated squared curvature](../../../../../triweight-density-minimizes-integrated-squared-curvature.md) under the specified constraints. Equality forces $e''=0$; a globally affine integrable difference of [probability density functions](../../../../../probability-density-function.md) is zero, so equality occurs only at $h=f_0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
