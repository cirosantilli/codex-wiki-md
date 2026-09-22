<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Jeffreys prior](../../../../../jeffreys-prior.md) is **invariant under smooth one-to-one reparameterization**. This means that applying the rule directly in a new parameter $\eta=h(\theta)$ gives the same [prior distribution](../../../../../prior-probability.md) as first constructing the rule for $\theta$ and then transforming its [prior density](../../../../../prior-density.md) by the change-of-variable formula.

More explicitly, for a differentiable invertible change of parameter with nonzero [derivative](../../../../../derivative.md),

$$
I_\eta(\eta)=I_\theta(\theta)\left(\frac{d\theta}{d\eta}\right)^2,
\qquad
\pi_{J,\eta}(\eta)\propto\sqrt{I_\eta(\eta)}
=\sqrt{I_\theta(\theta)}\left|\frac{d\theta}{d\eta}\right|.
$$

Thus $\pi_{J,\eta}(\eta)\,d\eta$ and $\pi_{J,\theta}(\theta)\,d\theta$ represent the same measure, up to the normalization constant. Invariance concerns the measure: the numerical values of the [prior densities](../../../../../prior-density.md) need not be equal in the two coordinates. The same change of variables then makes the [posterior distributions](../../../../../bayesian-posterior.md) agree. This is the [reparameterization invariance of Jeffreys prior](../../../../../reparameterization-invariance-of-jeffreys-prior.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
