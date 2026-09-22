<h1 id="27j/solution">Solution</h1>

↑ **Parent:** [27J](../27j.md)

A statistic is sufficient when the [conditional distribution](../../../../../conditional-distribution.md) of the observation given it does not depend on the parameter. It is minimal sufficient when it is, up to [null sets](../../../../../null-set.md), a [measurable function](../../../../../measurable-function.md) of every [sufficient statistic](../../../../../sufficient-statistic.md). For a dominated family, the likelihood-ratio criterion identifies two observations precisely when their [likelihood ratio](../../../../../likelihood-ratio.md) is independent of the parameter.

The Rao–Blackwell theorem says that conditioning a square-integrable [unbiased estimator](../../../../../unbiased-estimator.md) on a [sufficient statistic](../../../../../sufficient-statistic.md) preserves unbiasedness and cannot increase [variance](../../../../../variance-split.md). The Cramér–Rao bound for an [unbiased estimator](../../../../../unbiased-estimator.md) of scalar $\theta$ is $\operatorname{Var}_\theta\widehat\theta\ge1/I(\theta)$. It requires parameter-independent support, differentiability, interchange of differentiation and integration, and finite positive [Fisher information](../../../../../fisher-information-matrix.md). More generally the numerator is the square of the derivative of the estimand. The bound follows from $E_\theta[\widehat\theta\,\partial_\theta\log f]=1$ and Cauchy–Schwarz.

For the uniform sample, the joint [likelihood](../../../../../likelihood-function.md) is $\theta^{-n}\mathbf1_{\{0<x_i<\theta\ \forall i\}}$. Its dependence on the observations is through $T=\max_iX_i$, proving sufficiency. Two such [likelihoods](../../../../../likelihood-function.md) have parameter-independent ratio exactly when their maxima coincide, proving minimality. The density of $T$ is $nt^{n-1}/\theta^n$ on $(0,\theta)$. Unbiasedness of $h(T)$ says

$$
\int_0^\theta nh(t)t^{n-1}\,dt=\theta^{n+1}.
$$

Differentiating this absolutely [continuous](../../../../../continuous-function.md) identity gives $h(t)=(n+1)t/n$ [almost everywhere](../../../../../almost-everywhere.md). Conversely that function is unbiased. Every finite-variance [unbiased estimator](../../../../../unbiased-estimator.md), after Rao–Blackwellization, must therefore give this same function of $T$. Its [variance](../../../../../variance-split.md) cannot exceed that of any such estimator. Thus

$$
\boxed{\widehat\theta_{\rm MVU}=\frac{n+1}{n}\max_iX_i,\qquad\operatorname{Var}\widehat\theta_{\rm MVU}=\frac{\theta^2}{n(n+2)}.}
$$

The Cramér–Rao argument does not apply because the support depends on $\theta$; in particular differentiation of the support boundary invalidates the regular score identity.

## ↑ Ancestors (10)

1. [27J](../27j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
