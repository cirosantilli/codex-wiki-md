<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In [kernel density estimation](../../../../../kernel-density-estimation.md), take a [kernel for density estimation](../../../../../kernel-for-density-estimation.md) $K$ that is nonnegative, symmetric, and has integral one, finite $\mu_2(K)=\int u^2K(u)\,du>0$, and finite $R(K)=\int K(u)^2\,du$. Its [smoothing bandwidth](../../../../../smoothing-bandwidth.md) $h>0$ gives $K_h(u)=h^{-1}K(u/h)$ and the [kernel density estimator](../../../../../kernel-density-estimation.md)

$$
\widehat f_{h,K}(x)=\frac1n\sum_{i=1}^nK_h(x-X_i)
$$

from an [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md) sample with [probability density function](../../../../../probability-density-function.md) $f$. Nonnegativity and unit mass make the estimate itself a [probability density function](../../../../../probability-density-function.md). We compare [kernel for density estimation](../../../../../kernel-for-density-estimation.md) shapes by their optimized [mean integrated squared error](../../../../../integrated-mean-squared-error.md), rather than by their performance at an arbitrarily common numerical [smoothing bandwidth](../../../../../smoothing-bandwidth.md).

For the usual second-order theory, assume, for example, that $f$ belongs to the [Sobolev space](../../../../../sobolev-space-split.md) $H^2(\mathbb R)$ and $0<R(f'')<\infty$, and let $h\to0$, $nh\to\infty$. The [expectation](../../../../../expected-value.md) is the [convolution](../../../../../convolution.md) $K_h*f$. The vanishing first moment of the symmetric [kernel for density estimation](../../../../../kernel-for-density-estimation.md) and the integral [Taylor remainder](../../../../../taylor-remainder.md) give

$$
K_h*f-f=h^2\int_{\mathbb R}u^2K(u)\int_0^1(1-t)f''(\,\cdot-thu)\,dt\,du.
$$

Continuity of translations in the [L2 norm](../../../../../l2-norm.md), with domination by $u^2K(u)\|f''\|_2$, shows that $h^{-2}(K_h*f-f)\to\mu_2(K)f''/2$ in the [L2 norm](../../../../../l2-norm.md). Hence the integrated squared [bias of a kernel density estimator](../../../../../bias-of-a-kernel-density-estimator.md) is

$$
\|K_h*f-f\|_2^2=\frac14h^4\mu_2(K)^2R(f'')+o(h^4).
$$

By [independence](../../../../../independent-random-variables.md), the exact [integrated variance of a kernel density estimator](../../../../../integrated-variance-of-a-kernel-density-estimator.md) is

$$
\int\operatorname{Var}\{\widehat f_{h,K}(x)\}\,dx=\frac1n\left\{\frac{R(K)}h-R(K_h*f)\right\}.
$$

Indeed the integrated second moment of a single summand is $R(K)/h$, and its integrated squared [mean](../../../../../expected-value.md) is $R(K_h*f)$. The latter quantity is bounded by $R(f)$, by [Young's convolution inequality](../../../../../young-s-convolution-inequality.md), so its contribution is $O(n^{-1})$. The [bias-variance decomposition of mean squared error](../../../../../bias-variance-decomposition-of-mean-squared-error.md) therefore yields the leading criterion

$$
\operatorname{AMISE}_K(h)=\frac{R(K)}{nh}+\frac14h^4\mu_2(K)^2R(f'').
$$

This [asymptotic mean integrated squared error](../../../../../asymptotic-mean-integrated-squared-error.md) displays the [bias-variance tradeoff](../../../../../bias-variance-tradeoff.md): a small [smoothing bandwidth](../../../../../smoothing-bandwidth.md) increases integrated [variance](../../../../../variance-split.md), while a large one increases squared [bias of an estimator](../../../../../bias-of-an-estimator.md).

Differentiating the [asymptotic mean integrated squared error](../../../../../asymptotic-mean-integrated-squared-error.md) with respect to $h$ gives $-R(K)/(nh^2)+h^3\mu_2(K)^2R(f'')$. It changes sign once, from negative to positive, so its unique minimum is

$$
\boxed{h_{*,K}=\left\{\frac{R(K)}{n\mu_2(K)^2R(f'')}\right\}^{1/5}.}
$$

At this minimum the integrated [variance](../../../../../variance-split.md) term is four times the squared [bias of an estimator](../../../../../bias-of-an-estimator.md) term. Substitution gives

$$
\boxed{\inf_{h>0}\operatorname{AMISE}_K(h)=\frac54C(K)R(f'')^{1/5}n^{-4/5},\qquad C(K)=R(K)^{4/5}\mu_2(K)^{2/5}.}
$$

Thus the leading rate is $n^{-4/5}$, and the shape comparison reduces to minimizing $C(K)$.

There is an essential scale ambiguity: if $K_c(u)=c^{-1}K(u/c)$, then $\widehat f_{h,K_c}=\widehat f_{ch,K}$. Changing the scale of the [kernel for density estimation](../../../../../kernel-for-density-estimation.md) merely changes the numerical convention for the [smoothing bandwidth](../../../../../smoothing-bandwidth.md). Moreover

$$
R(K_c)=c^{-1}R(K),\qquad \mu_2(K_c)=c^2\mu_2(K),\qquad C(K_c)=C(K).
$$

A comparison at the same raw $h$ is therefore not a fair comparison of shape. One can normalize the second moment to one, but that does not make the optimal [smoothing bandwidth](../../../../../smoothing-bandwidth.md) independent of shape.

The [canonical kernel for density estimation](../../../../../canonical-kernel-for-density-estimation.md) instead chooses the unique scale

$$
\boxed{c_K=\left\{\frac{R(K)}{\mu_2(K)^2}\right\}^{1/5},\qquad K^{\mathrm{can}}(u)=c_K^{-1}K(u/c_K).}
$$

It satisfies $R(K^{\mathrm{can}})=\mu_2(K^{\mathrm{can}})^2=C(K)$, and so

$$
\operatorname{AMISE}_{K^{\mathrm{can}}}(h)=C(K)\left\{\frac1{nh}+\frac14h^4R(f'')\right\}.
$$

Consequently **all canonical kernels share the same leading optimal bandwidth $h_*=[nR(f'')]^{-1/5}$**. Only the multiplicative constant $C(K)$ depends on shape. This is precisely the separation of shape choice and scale choice that makes the [canonical kernel](../../../../../canonical-kernel-for-density-estimation.md) normalization useful. For an original unscaled [kernel for density estimation](../../../../../kernel-for-density-estimation.md), its corresponding optimal [smoothing bandwidth](../../../../../smoothing-bandwidth.md) is $c_Kh_*$.

To prove optimal shape, scale a candidate [kernel for density estimation](../../../../../kernel-for-density-estimation.md) to have second moment one. Let $B=\sqrt5$ and

$$
E(u)=\frac{3}{4B^3}(B^2-u^2)_+=\frac3{4\sqrt5}\left(1-\frac{u^2}5\right)_+.
$$

Direct integration gives $\int E=1$, $\int u^2E(u)\,du=B^2/5=1$, and $R(E)=3/(5B)$. Thus $E$ is a rescaled [Epanechnikov kernel](../../../../../epanechnikov-kernel.md). For any admissible $K$ with the same mass and second moment,

$$
\int_{\mathbb R}(B^2-u^2)(K-E)\,du=0.
$$

Outside $[-B,B]$, $E=0$ and $(B^2-u^2)K\leq0$, because $K\geq0$. The integral inside $[-B,B]$ is therefore nonnegative, and multiplying by $3/(4B^3)$ gives $\int E(K-E)\geq0$. Expanding the square now proves

$$
R(K)-R(E)=\int(K-E)^2+2\int E(K-E)\geq0.
$$

Equality forces $K=E$ almost everywhere. At fixed second moment, minimizing $R(K)$ is equivalent to minimizing $C(K)$. Since $C(K)$ is scale invariant, this proves the [optimality of the Epanechnikov kernel](../../../../../optimality-of-the-epanechnikov-kernel.md) over all nonnegative symmetric second-order [kernels for density estimation](../../../../../kernel-for-density-estimation.md), including the equality case up to rescaling.

In its usual scale, the optimal [Epanechnikov kernel](../../../../../epanechnikov-kernel.md) is

$$
\boxed{K_E(u)=\frac34(1-u^2)\mathbf1_{\{|u|\leq1\}},\qquad \mu_2(K_E)=\frac15,\qquad R(K_E)=\frac35.}
$$

Its canonical scale is $c_E=15^{1/5}$, giving

$$
K_E^{\mathrm{can}}(u)=\frac3{4\,15^{1/5}}\left(1-\frac{u^2}{15^{2/5}}\right)_+.
$$

The optimal [Epanechnikov kernel](../../../../../epanechnikov-kernel.md) shape is therefore a truncated parabola, rather than a particular support radius. The [canonical kernel](../../../../../canonical-kernel-for-density-estimation.md) and unit-second-moment version represent the same shape but different scale conventions.

The numerical gains over other reasonable [kernels for density estimation](../../../../../kernel-for-density-estimation.md) are modest. Define [asymptotic relative efficiency](../../../../../asymptotic-relative-efficiency.md) against the optimal [Epanechnikov kernel](../../../../../epanechnikov-kernel.md) by the sample-size fraction giving the same optimized leading [mean integrated squared error](../../../../../integrated-mean-squared-error.md):

$$
\operatorname{Eff}(K)=\left\{\frac{C(K_E)}{C(K)}\right\}^{5/4}=\frac{R(K_E)\sqrt{\mu_2(K_E)}}{R(K)\sqrt{\mu_2(K)}}\leq1.
$$

For the [Gaussian density kernel](../../../../../gaussian-density-kernel.md) $K_N(u)=(2\pi)^{-1/2}e^{-u^2/2}$, $R(K_N)=1/(2\sqrt\pi)$ and $\mu_2(K_N)=1$, so its efficiency is $6\sqrt\pi/(5\sqrt5)\simeq0.9512$. For the [uniform smoothing kernel](../../../../../uniform-smoothing-kernel.md) $K_U(u)=\tfrac12\mathbf1_{\{|u|\leq1\}}$, $R(K_U)=1/2$ and $\mu_2(K_U)=1/3$, giving efficiency $6\sqrt3/(5\sqrt5)\simeq0.9295$. The [Gaussian density kernel](../../../../../gaussian-density-kernel.md) is infinitely smooth, whereas the optimal [Epanechnikov kernel](../../../../../epanechnikov-kernel.md) has compact support and allows each observation to affect only a finite window. Such computational and smoothness considerations may outweigh a small leading-efficiency difference.

In practice $R(f'')$ is unknown. A [plug-in estimator](../../../../../plug-in-estimator.md) estimates this roughness functional from a pilot estimate of the [second derivative](../../../../../second-derivative.md) and substitutes it into the optimal [smoothing bandwidth](../../../../../smoothing-bandwidth.md) formula. Alternatively, [Leave-one-out cross-validation](../../../../../leave-one-out-cross-validation.md) minimizes

$$
\operatorname{CV}(h)=\int\widehat f_{h,K}(x)^2\,dx-\frac2n\sum_{i=1}^n\widehat f_{-i,h,K}(X_i),
$$

where $\widehat f_{-i,h,K}$ uses the other $n-1$ observations. By [independence](../../../../../independent-random-variables.md), the [expectation](../../../../../expected-value.md) of the second term is $2\int(K_h*f)f$, so $\mathbb E\operatorname{CV}(h)=\operatorname{MISE}(h)-R(f)$. Thus it targets integrated error without knowing $f$. The choice of [smoothing bandwidth](../../../../../smoothing-bandwidth.md) remains important: even for the optimal [Epanechnikov kernel](../../../../../epanechnikov-kernel.md), setting $h=t h_{*,K}$ multiplies the leading minimum error by $(4t^{-1}+t^4)/5$.

The preceding optimum concerns nonnegative second-order [kernels for density estimation](../../../../../kernel-for-density-estimation.md) and twice-smooth densities on the real line. Signed [kernels of order ell](../../../../../kernel-of-order-ell.md) can cancel higher moments for smoother densities and yield different rates, but may produce negative density estimates. A support boundary or a density jump also requires separate [bias of a kernel density estimator](../../../../../bias-of-a-kernel-density-estimator.md) analysis. These settings do not contradict the proved second-order [optimality of the Epanechnikov kernel](../../../../../optimality-of-the-epanechnikov-kernel.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
