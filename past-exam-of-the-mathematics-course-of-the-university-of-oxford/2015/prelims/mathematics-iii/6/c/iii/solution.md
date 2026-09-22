<h1 id="6/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [probability density function](../../../../../../../probability-density-function.md) must integrate to one, so

$$
1=\frac1{\sqrt\pi}\int_0^\infty y^{-1/2}e^{-y}\,dy,\qquad \boxed{\int_0^\infty t^{-1/2}e^{-t}\,dt=\sqrt\pi.}
$$

Also, [linearity of expectation](../../../../../../../linearity-of-expectation.md) and the [mean](../../../../../../../expected-value-split.md) and [variance](../../../../../../../variance-split.md) of the [standard normal distribution](../../../../../../../standard-normal-distribution.md) give

$$
\mathbb E[Y]=\frac12\mathbb E[Z^2]=\frac12\left(\operatorname{var}(Z)+(\mathbb E[Z])^2\right)=\frac12.
$$

Using the [probability density function](../../../../../../../probability-density-function.md) to compute this [expected value](../../../../../../../expected-value-split.md) gives

$$
\frac12=\frac1{\sqrt\pi}\int_0^\infty y^{1/2}e^{-y}\,dy,\qquad \boxed{\int_0^\infty t^{1/2}e^{-t}\,dt=\frac{\sqrt\pi}{2}.}
$$

These are the values $\Gamma(1/2)$ and $\Gamma(3/2)$ of the [gamma function](../../../../../../../gamma-function.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
