<h1 id="4/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Recognize the integrand as a [Gaussian scale mixture](../../../../../../../gaussian-scale-mixture.md). If $R$ has the unit [Rayleigh distribution](../../../../../../../rayleigh-distribution.md) and $Z$ is an independent [standard normal distribution](../../../../../../../standard-normal-distribution.md) variable, then the conditional density of $RZ$ given $R=r$ is $(\sqrt{2\pi}r)^{-1}e^{-x^2/(2r^2)}$. Multiplying by the radius density gives

$$
\int_0^\infty\frac1{\sqrt{2\pi}r}e^{-x^2/(2r^2)}\,r e^{-r^2/2}\,dr
=\frac1{\sqrt{2\pi}}\int_0^\infty e^{-(x^2+r^4)/(2r^2)}\,dr=g(x).
$$

Thus use $U_1$ for the independent radius and $U_2,U_3$ for the normal output of the [Box-Muller transform](../../../../../../../box-muller-transform.md):

$$
\boxed{X=\sqrt{-2\log U_1}\,\sqrt{-2\log U_2}\cos(2\pi U_3).}
$$

The mixture argument also proves that $g$ integrates to one, by the [Tonelli theorem](../../../../../../../tonelli-theorem.md). As a check, $R^2$ is exponential of rate $1/2$, so the [characteristic function](../../../../../../../characteristic-function.md) of $RZ$ is $\mathbb E e^{-t^2R^2/2}=1/(1+t^2)$. This is the [Rayleigh-normal scale mixture](../../../../../../../rayleigh-normal-scale-mixture.md), with [Laplace distribution](../../../../../../../laplace-distribution.md) density $e^{-|x|}/2$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
