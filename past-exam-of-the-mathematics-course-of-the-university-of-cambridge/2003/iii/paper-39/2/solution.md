<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $Y=(\log X-\mu)/\sigma$ and write $\phi$ for the [standard normal density](../../../../../standard-normal-density.md), with $\sigma>0$. The [change of variables](../../../../../change-of-variables-formula.md) converts the density integral into

$$
\int_a^b x^kf(x)\,dx=e^{k\mu}\int_{(\log a-\mu)/\sigma}^{(\log b-\mu)/\sigma}e^{k\sigma y}\phi(y)\,dy.
$$

Complete the square using $e^{k\sigma y}\phi(y)=e^{k^2\sigma^2/2}\phi(y-k\sigma)$. Integration gives the [truncated lognormal moment](../../../../../truncated-lognormal-moment.md)

$$
\boxed{\int_a^b x^kf(x)\,dx=e^{k\mu+k^2\sigma^2/2}\left[\Phi\!\left(\frac{\log b-\mu-k\sigma^2}{\sigma}\right)-\Phi\!\left(\frac{\log a-\mu-k\sigma^2}{\sigma}\right)\right].}
$$

Here $\Phi$ is the [standard normal distribution function](../../../../../standard-normal-distribution-function.md); take $\log0=-\infty$ and $\log\infty=\infty$. The identity holds for every real $k$, including the full-interval limits, because the shifted Gaussian integral remains finite.

The [limited excess of loss reinsurance](../../../../../limited-excess-of-loss-reinsurance.md) payment is $L(X)=\min\{(X-M)_+,A\}$. It is zero below $M$, equals $X-M$ for $M<X<M+A$, and equals $A$ above $M+A$. Since the [lognormal distribution](../../../../../log-normal-distribution.md) has a continuous density,

$$
\mathbb E L(X)=\int_M^{M+A}(x-M)f(x)\,dx+A\mathbb P(X>M+A).
$$

Put $d_j(t)=(\log t-\mu-j\sigma^2)/\sigma$, $j=0,1$, and $\overline\Phi=1-\Phi$. Applying the moment identity with $k=1$ and $k=0$ gives the [conditional lognormal layer recovery](../../../../../conditional-lognormal-layer-recovery.md)

$$
\boxed{C(\mu,\sigma;M,A)=\frac{e^{\mu+\sigma^2/2}[\Phi(d_1(M+A))-\Phi(d_1(M))]-M[\Phi(d_0(M+A))-\Phi(d_0(M))]+A\overline\Phi(d_0(M+A))}{\overline\Phi(d_0(M))}.}
$$

The denominator is $\mathbb P(X>M)$, and payments outside that event are zero. The three numerator terms are respectively the truncated first moment, the attachment subtracted from partial payments, and the capped payments on claims above the layer. This proves the conditional expectation including the limit on each reinsurer payment.

For [claims inflation](../../../../../claims-inflation.md) by $h=1.1$, set $X_h=hX$. Its log-mean is $\mu_h=\mu+\log h$ and its log-standard-deviation stays $\sigma$. The attachment and payment limit stay fixed. Therefore the requested new conditional mean is

$$
\boxed{\mathbb E[\min\{(1.1X-M)_+,A\}\mid1.1X>M]=C(\mu+\log1.1,\sigma;M,A).}
$$

Explicitly, in the preceding fraction replace $d_j(t)$ by $d_j^{(h)}(t)=(\log t-\mu-\log1.1-j\sigma^2)/\sigma$ and replace $e^{\mu+\sigma^2/2}$ by $1.1e^{\mu+\sigma^2/2}$. Equivalently, [claims inflation of a fixed reinsurance layer](../../../../../claims-inflation-of-a-fixed-reinsurance-layer.md) gives

$$
\boxed{C(\mu+\log1.1,\sigma;M,A)=1.1\,C(\mu,\sigma;M/1.1,A/1.1),}
$$

because $L_{M,A}(hX)=hL_{M/h,A/h}(X)$ and the new conditioning event is $X>M/h$. Merely multiplying the original conditional mean by $1.1$ would omit both of these threshold changes.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
