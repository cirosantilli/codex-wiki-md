<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Saddlepoint approximation methods retain the nonquadratic shape of a distribution through its [cumulant-generating function](../../../../../../cumulant-generating-function.md). Suppose $X_1,\ldots,X_n$ are independent and identically distributed, $K(t)=\log E(e^{tX_1})$ is finite on an open interval containing zero, and $K''>0$. For an interior target mean $x$, solve the saddlepoint equation $K'(t)=x$. Introduce [exponential tilting](../../../../../../exponential-tilting.md) by

$$
dP_t(y)=e^{ty-K(t)}\,dP(y).
$$

Under the tilted distribution the mean and [variance](../../../../../../variance-split.md) are $K'(t)=x$ and $K''(t)$. For the product sample the [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) is $e^{t\sum_iX_i-nK(t)}$. Consequently the exact [density](../../../../../../density.md) relation for the [sample mean](../../../../../../sample-mean.md) is

$$
f_{\overline X}(x)=e^{n(K(t)-tx)}f_{\overline X,t}(x).
$$

A local central limit approximation to the tilted [density](../../../../../../density.md) at its own mean gives $f_{\overline X,t}(x)\simeq\sqrt{n/(2\pi K''(t))}$. Hence

$$
\boxed{f_{\overline X}(x)\simeq\sqrt{\frac n{2\pi K''(t)}}\exp\{n(K(t)-tx)\},\qquad K'(t)=x.}
$$

For the sum $S_n$, the equivalent expression is $f_{S_n}(s)\simeq e^{nK(t)-ts}/\sqrt{2\pi nK''(t)}$, with $K'(t)=s/n$. Under the usual smooth nonlattice [density](../../../../../../density.md) conditions this approximation has relative error of order $n^{-1}$ for a fixed interior target. In the tilted [Edgeworth expansion](../../../../../../edgeworth-series.md) the order $n^{-1/2}$ odd term vanishes at the mean. The exponent retains the Legendre-transform rate $I(x)=tx-K(t)$, rather than a quadratic Taylor approximation to that rate, explaining the useful tail and skewness behavior. Normalization is not automatic, and accuracy statements need their regularity and range restrictions.

For a [normal distribution](../../../../../../normal-distribution.md), $K(t)=\mu t+\sigma^2t^2/2$ and $t=(x-\mu)/\sigma^2$. Substitution recovers exactly the normal [density](../../../../../../density.md) of the [sample mean](../../../../../../sample-mean.md). For an [exponential distribution](../../../../../../exponential-distribution.md) of rate $\lambda$, $K(t)=-\log(1-t/\lambda)$, $t=\lambda-1/x$ and $K''(t)=x^2$. The approximation becomes

$$
\sqrt{\frac n{2\pi}}\,\lambda^n e^n x^{n-1}e^{-n\lambda x},\qquad x>0.
$$

It has exactly the gamma [density](../../../../../../density.md) shape. Replacing its leading constant by the exact [normalizing constant](../../../../../../normalizing-constant.md) makes it exact, illustrating why exactness of shape and exactness of the unnormalized approximation are separate questions.

For a vector [sample mean](../../../../../../sample-mean.md), tilt by $e^{t^{\mathsf T}y-K(t)}$, solve $\nabla K(t)=x$, and use the local multivariate normal [density](../../../../../../density.md) at the tilted mean. This gives

$$
f_{\overline X}(x)\simeq\frac{(n/(2\pi))^{d/2}}{\sqrt{\det K''(t)}}\exp\{n(K(t)-t^{\mathsf T}x)\}.
$$

Joint and marginal saddlepoint densities can also be divided to approximate conditional densities, for example after conditioning on a nuisance [sufficient statistic](../../../../../../sufficient-statistic.md). The [p\* approximation](../../../../../../p-star-approximation.md) uses [likelihood](../../../../../../likelihood-function.md) and fitted-information coordinates to obtain a closely related approximation to a [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md)'s [density](../../../../../../density.md), usually conditional on an [ancillary statistic](../../../../../../ancillary-statistic.md).

Tail probabilities need a corresponding integration approximation. The [Lugannani-Rice saddlepoint tail approximation](../../../../../../lugannani-rice-saddlepoint-tail-approximation.md) uses

$$
w=\operatorname{sgn}(t)\sqrt{2n\{tx-K(t)\}},\qquad u=t\sqrt{nK''(t)},
$$

and gives

$$
\boxed{\Pr(\overline X\le x)\simeq\Phi(w)+\phi(w)\left(\frac1w-\frac1u\right).}
$$

Here $\Phi,\phi$ are the standard [normal distribution](../../../../../../normal-distribution.md) functions. The upper-tail correction has the opposite sign: $1-\Phi(w)+\phi(w)(1/u-1/w)$. Inverting a [cumulative distribution function](../../../../../../cumulative-distribution-function.md) introduces a pole in addition to the [density](../../../../../../density.md)'s saddlepoint; treating both supplies the correction term, which is why simply integrating a normal approximation at the untilted mean is less accurate. At $x=K'(0)$ the apparent singularities cancel. With $v=K''(0)$ and $k=K'''(0)$, expansions give $w=t\sqrt{nv}(1+kt/(3v)+O(t^2))$ and $u=t\sqrt{nv}(1+kt/(2v)+O(t^2))$, so $1/w-1/u\to k/(6\sqrt n\,v^{3/2})$. For the [normal distribution](../../../../../../normal-distribution.md) the correction is zero everywhere.

These methods require care for lattice distributions, where summation and lattice corrections replace the [density](../../../../../../density.md) inversion, and near boundaries or singular [covariance](../../../../../../covariance.md) matrices. A distribution with no [moment-generating function](../../../../../../moment-generating-function.md) in a neighborhood of zero does not satisfy the starting assumptions. A successful saddlepoint approximation is therefore a structured refinement of regular asymptotic inference, not a formula guaranteed uniformly in every tail or for every model.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
