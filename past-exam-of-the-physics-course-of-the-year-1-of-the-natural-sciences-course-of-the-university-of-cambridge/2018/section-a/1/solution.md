<h1 id="section-a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the same massless [spring](../../../../spring.md) of [spring constant](../../../../spring-constant.md) $k$, [Hooke's law](../../../../hooke-s-law.md) gives the vertical [simple harmonic motion](../../../../simple-harmonic-motion.md) about the displaced [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) position:

$$
\nu_i=\frac1{2\pi}\sqrt{\frac{k}{m_i}},\qquad
R=\frac{m_1}{m_2}=\left(\frac{\nu_2}{\nu_1}\right)^2.
$$

Gravity shifts the [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) extension but does not change this [frequency](../../../../frequency.md). Use the measured [sample means](../../../../sample-mean.md) in the ratio estimate. For small measurement errors, [logarithmic differentiation](../../../../logarithmic-differentiation.md) gives

$$
\frac{dR}{R}=2\frac{d\nu_2}{\nu_2}-2\frac{d\nu_1}{\nu_1}.
$$

Assuming the two frequency estimates have [independent](../../../../independent-random-variables.md) errors, their [variances](../../../../variance-split.md) add. Writing $\epsilon=\delta\nu/\overline\nu$ for their common fractional [standard uncertainty](../../../../standard-uncertainty.md), [monomial uncertainty propagation](../../../../monomial-uncertainty-propagation.md) yields

$$
\left(\frac{\sigma(R)}R\right)^2\simeq4\epsilon^2+4\epsilon^2,
\qquad
\boxed{\frac{\sigma(R)}R\simeq\sqrt8\,\frac{\delta\nu}{\overline\nu}.}
$$

This is a first-order uncertainty formula, rather than an exact identity for an arbitrary noisy ratio. It assumes that errors in the two measured [frequencies](../../../../frequency.md) have zero [covariance](../../../../covariance.md).

There is a statistical distinction in the wording: the [standard deviation](../../../../standard-deviation.md) of individual repetitions is not the [standard error](../../../../standard-error.md) of their [sample mean](../../../../sample-mean.md). If the supplied $\sigma(\nu_i)$ describes individual trials, the frequency means have errors $\sigma(\nu_i)/\sqrt n$, and the ratio formed from those means instead satisfies

$$
\boxed{\frac{\sigma(R_{\rm means})}{R_{\rm means}}\simeq
\sqrt{\frac8n}\,\frac{\delta\nu}{\overline\nu}.}
$$

Thus the printed formula describes either a single-pair ratio or a convention in which $\delta\nu$ already denotes the uncertainty of each averaged [frequency](../../../../frequency.md). Under either consistent interpretation, [independent](../../../../independent-random-variables.md) repeated measurements reduce statistical error in proportion to $n^{-1/2}$. Halving it requires **$4n$ trials in total for each mass, or $3n$ additional trials**. Repetition alone does not reduce a fixed [systematic error](../../../../systematic-error.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Section A](../../section-a.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
