<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In a [parametric statistical model](../../../../../parametric-statistical-model.md) $\{P_\theta:\theta\in\Theta\}$, the [likelihood function](../../../../../likelihood-function.md) $L(\theta;y)$ measures the relative support given by the observed sample for different parameter values. [Maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md) supplies a point estimate; the sampling distributions of suitable [statistics](../../../../../statistic.md) calibrate significance tests and [confidence intervals](../../../../../confidence-interval.md). A [sufficient statistic](../../../../../sufficient-statistic.md) retains all parameter-dependent information in the [likelihood function](../../../../../likelihood-function.md), so one first seeks a reduction to such a [statistic](../../../../../statistic.md) rather than discarding information arbitrarily.

The characteristic conditioning principle in [Fisherian conditional inference](../../../../../fisherian-conditional-inference.md) is to calibrate inference conditional on the observed value of an [ancillary statistic](../../../../../ancillary-statistic.md). With no [nuisance parameter](../../../../../nuisance-parameter.md), a [statistic](../../../../../statistic.md) $A$ is ancillary when its law is the same for every $\theta$. Its observed value can nevertheless describe the experimental configuration or precision. Conditional inference uses $\mathcal L_\theta(T\mid A=a)$ for an informative [statistic](../../../../../statistic.md) $T$, with $a$ the observed ancillary value. Since the marginal law of $A$ does not depend on $\theta$, conditioning leaves the parameter-dependent [likelihood](../../../../../likelihood-function.md) factor unchanged, while potentially changing the appropriate repeated-sampling reference distribution. Conditioning on a continuous $A$ means using a [regular conditional distribution](../../../../../regular-conditional-distribution.md), rather than dividing by $\mathbb P(A=a)$.

With parameters $(\psi,\lambda)$, where $\psi$ is the target and $\lambda$ a [nuisance parameter](../../../../../nuisance-parameter.md), a fully [ancillary statistic](../../../../../ancillary-statistic.md) has a law independent of both. A [partial ancillary statistic](../../../../../partial-ancillary-statistic.md) for $\psi$ may have a law depending on $\lambda$ but not on $\psi$. To eliminate $\lambda$ by conditioning, one needs the actual conditional law of the informative [statistic](../../../../../statistic.md) to be free of $\lambda$; partial ancillarity by itself does not guarantee this. For example, if independent counts have [Poisson distributions](../../../../../poisson-distribution.md) with means $\lambda\psi$ and $\lambda(1-\psi)$, their total $N$ has [Poisson distribution](../../../../../poisson-distribution.md) with mean $\lambda$, independent of $\psi$. The first count conditional on $N=m$ has [binomial distribution](../../../../../binomial-distribution.md) with parameters $(m,\psi)$. Conditioning removes the nuisance intensity $\lambda$ exactly. More generally, nuisance-free [pivotal quantities](../../../../../pivotal-quantity.md) or [conditional likelihoods](../../../../../conditional-likelihood.md) can be used where available; there is no universal conditioning device that removes every [nuisance parameter](../../../../../nuisance-parameter.md).

For a concrete example of [non-uniqueness of maximal ancillary statistics](../../../../../non-uniqueness-of-maximal-ancillary-statistics.md), consider one observed pair $(U,V)\in\{0,1\}^2$, with

$$
P_\theta(0,0)=P_\theta(1,1)=\frac\theta2,\qquad
P_\theta(0,1)=P_\theta(1,0)=\frac{1-\theta}{2},\qquad0<\theta<1.
$$

Both $U$ and $V$ have [Bernoulli distribution](../../../../../bernoulli-distribution.md) with success probability $1/2$, independent of $\theta$, so each is an [ancillary statistic](../../../../../ancillary-statistic.md). Their generated partitions are different and incomparable. Moreover, each is maximal: refining either two-point cell singles out a point whose probability is $\theta/2$ or $(1-\theta)/2$, which is parameter-dependent. Their joint [statistic](../../../../../statistic.md) is not ancillary, since $P_\theta(U=V)=\theta$. Thus there is no common finer ancillary partition that reconciles the two choices. The conditional laws differ as labelled experiments: $P_\theta(V=U\mid U)=\theta$ and $P_\theta(U=V\mid V)=\theta$, but they condition on different observed information. This illustrates why “condition on a maximal ancillary” need not specify a unique procedure.

For the [location-scale family](../../../../../location-scale-family.md), write $Y_i=\mu+\sigma Z_i$, where the $Z_i$ are independent with the fixed density $f_0$. Let $s_Z^2=n^{-1}\sum_i(Z_i-\bar Z)^2$. The transformation gives

$$
\widehat\mu=\bar Y=\mu+\sigma\bar Z,\qquad
\widehat\sigma=\sigma s_Z,
$$

and therefore

$$
\boxed{A_i=\frac{Y_i-\widehat\mu}{\widehat\sigma}
=\frac{Z_i-\bar Z}{s_Z}.}
$$

For $n\geq2$, $s_Z>0$ [almost surely](../../../../../almost-sure-convergence.md), because an independent sample from a density has probability zero of all observations coinciding. The right side depends only on a sample from the fixed base law, so the entire vector $A$ has a law independent of $(\mu,\sigma)$: $\boxed{A\text{ is ancillary}.}$ No finite population mean or [variance](../../../../../variance-split.md) is needed for this algebraic argument. With one observation the displayed standardization is undefined, so at least two observations are implicitly required.

The pair $(\widehat\mu,\widehat\sigma)$ together with $A$ reconstructs the full sample through $Y_i=\widehat\mu+\widehat\sigma A_i$. Thus [conditional inference in a location-scale family](../../../../../conditional-inference-in-a-location-scale-family.md) uses

$$
\boxed{\mathcal L_{\mu,\sigma}(\widehat\mu,\widehat\sigma\mid A=a),}
$$

where $a$ is the observed residual configuration. Equivalently one can use the parameter-free conditional law of $((\widehat\mu-\mu)/\sigma,\widehat\sigma/\sigma)$ given $A=a$. To see this explicitly, the centered residual subspace has dimension $n-1$, so its radial coordinate $t=\widehat\sigma$ contributes a [Jacobian determinant](../../../../../jacobian-determinant.md) factor proportional to $t^{n-2}$. The [conditional density](../../../../../conditional-density.md) of $\widehat\mu=m$, $\widehat\sigma=t>0$ is therefore proportional to

$$
t^{n-2}\sigma^{-n}\prod_{i=1}^nf_0\!\left(\frac{m+ta_i-\mu}{\sigma}\right).
$$

Setting $u=(m-\mu)/\sigma$ and $v=t/\sigma$ gives a [conditional density](../../../../../conditional-density.md) proportional to $v^{n-2}\prod_i f_0(u+va_i)$, with no unknown parameter. The normalizing factor can depend on $a$, but not on $\mu$ or $\sigma$. These statements concern almost every attainable ancillary value.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
