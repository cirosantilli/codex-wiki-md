<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the usual probability-kernel convention: $K\ge0$, $\int K=1$, and $K\in L^2$, in addition to symmetry and [compact support](../../../../../compact-support.md). These conditions are needed for the stated finite bound; symmetry and [compact support](../../../../../compact-support.md) by themselves do not impose normalization or nonnegativity. Interpret the differentiability assumption in the usual [Sobolev space](../../../../../sobolev-space-split.md) sense $f\in H^2(\mathbb R)$, or assume classical regularity sufficient for the integral [Taylor remainder](../../../../../taylor-remainder.md). The [kernel density estimator](../../../../../kernel-density-estimation.md) is

$$
\widehat f_h(x)=\frac1{nh}\sum_{i=1}^nK\!\left(\frac{x-X_i}{h}\right),\qquad K_h(x)=h^{-1}K(x/h),
\qquad \mathbb E\widehat f_h=K_h*f.
$$

The [bias-variance decomposition of mean squared error](../../../../../bias-variance-decomposition-of-mean-squared-error.md), followed by [Tonelli theorem](../../../../../tonelli-theorem.md), yields

$$
\mathbb E\|\widehat f_h-f\|_2^2
=\int\operatorname{Var}(\widehat f_h(x))\,dx+\|K_h*f-f\|_2^2.
$$

[Independence](../../../../../independent-random-variables.md) and a [change of variables](../../../../../change-of-variables-formula.md) give the exact [integrated variance of a kernel density estimator](../../../../../integrated-variance-of-a-kernel-density-estimator.md)

$$
\int\operatorname{Var}(\widehat f_h(x))\,dx
=\frac1n\left(\frac{\|K\|_2^2}{h}-\|K_h*f\|_2^2\right)
\le\frac{\|K\|_2^2}{nh}.
$$

All changes of integration order are justified either by nonnegativity or by the displayed finite integrals.

For the [bias of a kernel density estimator](../../../../../bias-of-a-kernel-density-estimator.md), symmetry gives $\int uK(u)\,du=0$. Taylor's integral remainder, with translations understood in $L^2$, gives

$$
f(x-hu)-f(x)+hu f'(x)=h^2u^2\int_0^1(1-t)f''(x-thu)\,dt.
$$

The [Minkowski inequality](../../../../../minkowski-inequality.md) and translation invariance of the [L2 norm](../../../../../l2-norm.md) imply

$$
\|f(\cdot-hu)-f+hu f'\|_2\le\frac{h^2u^2}{2}\|f''\|_2,
\qquad
\|K_h*f-f\|_2\le\frac{h^2}{2}\mu_2(K)\|f''\|_2,
$$

where $\mu_2(K)=\int u^2K(u)\,du$. Consequently we obtain the slightly stronger conclusion

$$
\boxed{\mathbb E\|\widehat f_h-f\|_2^2\le
\frac{\|K\|_2^2}{nh}+\frac14h^4\mu_2(K)^2\|f''\|_2^2.}
$$

Since $1/4\le1/3$, this proves the requested bound. For signed kernels, the same argument has $\int u^2|K(u)|\,du$ in place of $\mu_2(K)$; the printed bound is not generally justified merely by signed-kernel symmetry. For example, let $U_a=(2a)^{-1}\mathbf1_{[-a,a]}$ and $K=(4/3)U_1-(1/3)U_2$. This symmetric compactly supported signed kernel has integral one and $\mu_2(K)=0$, but its fourth moment is nonzero. For a normal density its convolution has nonzero bias at any fixed positive bandwidth. Sending $n\to\infty$ would therefore contradict a bound containing only the integrated variance term.

Writing the requested bound as $A/(nh)+Bh^4$, differentiation gives $h_*=(A/(4Bn))^{1/5}$ when $B>0$. Thus **$h\asymp n^{-1/5}$ gives [mean integrated squared error](../../../../../integrated-mean-squared-error.md) of order $n^{-4/5}$**. With the sharper constant one instead has $h_*=(\|K\|_2^2/(n\mu_2(K)^2\|f''\|_2^2))^{1/5}$; the rate is identical.

A direct heuristic for $J_2(f)=\|f''\|_2^2$ is to choose a twice differentiable pilot kernel $L$, estimate $f''$ by the [second derivative kernel density estimator](../../../../../second-derivative-kernel-density-estimator.md)

$$
\widehat f_b''(x)=\frac1{nb^3}\sum_i L''\!\left(\frac{x-X_i}{b}\right),
$$

and integrate its square. Its integrated [variance](../../../../../variance-split.md) contains a diagonal term $\|L''\|_2^2/(nb^5)$, which should not be mistaken for the target. A useful corrected [U-statistic](../../../../../u-statistic.md) removes that diagonal:

$$
\widehat J_{2,b}=\frac1{n(n-1)b^5}\sum_{i\ne j}A\!\left(\frac{X_i-X_j}{b}\right),
\qquad A(v)=\int L''(t)L''(t+v)\,dt.
$$

Its [expectation](../../../../../expected-value.md) is $\|L_b*f''\|_2^2$. Thus smoothing [bias of an estimator](../../../../../bias-of-an-estimator.md), rather than the diagonal contribution, remains. For a smooth compactly supported probability pilot kernel, the same variance calculation gives

$$
\mathbb E\|\widehat f_b''-f''\|_2^2\le\frac{\|L''\|_2^2}{nb^5}+\|L_b*f''-f''\|_2^2.
$$

The second term tends to zero because convolution with a shrinking probability kernel approximates every $L^2$ function. Thus $b\to0$ and $nb^5\to\infty$ make the raw squared pilot estimate consistent for the [quadratic density derivative functional](../../../../../quadratic-density-derivative-functional.md). If $Q_b=\int(\widehat f_b'')^2$, then

$$
\widehat J_{2,b}=\frac n{n-1}\left(Q_b-\frac{\|L''\|_2^2}{nb^5}\right),
$$

so the diagonal-corrected [U-statistic](../../../../../u-statistic.md) is consistent under the same choice. Consistency already uses the assumed $f''\in L^2$; the additional third-derivative hypothesis is relevant to more ambitious rate heuristics.

**Three bounded continuous [derivatives](../../../../../derivative.md) do not justify a general root-$n$ estimation rate for $J_2$.** For a smooth perturbation $a$ with [compact support](../../../../../compact-support.md), the [directional derivative](../../../../../directional-derivative.md) is

$$
\left.\frac{d}{dt}J_2(f+ta)\right|_{t=0}
=2\int f''a''=2\int f^{(4)}a,
$$

where the last expression requires a fourth [derivative](../../../../../derivative.md) in the appropriate weak sense. A regular root-$n$ argument would need an [influence function](../../../../../influence-function.md) proportional to $f^{(4)}$, with finite [variance](../../../../../variance-split.md) under $f$. Three [derivatives](../../../../../derivative.md) do not supply that condition.

For a more quantitative heuristic, impose the additional assumption $f\in H^\beta$, use a smooth Fourier cutoff of width $1/b$, and estimate the quadratic functional by its off-diagonal [U-statistic](../../../../../u-statistic.md). The tail [bias of an estimator](../../../../../bias-of-an-estimator.md) is $O(b^{2(\beta-2)})$ because the [Plancherel theorem](../../../../../plancherel-theorem.md) weights this functional by frequency to the fourth power. The degenerate part of its standard deviation is $O(n^{-1}b^{-9/2})$: the squared $L^2$ norm of the quadratic kernel scales as $b^{-9}$. At $\beta=3$, these two terms balance at $b\asymp n^{-2/13}$ and have size $n^{-4/13}$, already slower than $n^{-1/2}$; any additional first-order [variance](../../../../../variance-split.md) cannot improve that balance. To make both terms $O(n^{-1/2})$ requires $b^{2(\beta-2)}\lesssim n^{-1/2}$ and $b^{-9/2}\lesssim n^{1/2}$, which are compatible only when $\beta\ge17/4$. This is an illustrative smoothness calculation under extra Sobolev and moment assumptions, not a rate theorem asserted solely from bounded third [derivatives](../../../../../derivative.md). Particular much smoother [probability density functions](../../../../../probability-density-function.md) may of course permit root-$n$ estimation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
