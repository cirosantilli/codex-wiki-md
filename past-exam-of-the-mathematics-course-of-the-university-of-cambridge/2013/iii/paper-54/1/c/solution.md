<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The instantaneous [kinematic viscosity](../../../../../../kinematic-viscosity.md) law is $\bar\nu(r,\Sigma)$, with no explicit constitutive memory. Expand its transported quantity at the possibly evolving background:

$$
\bar\nu(r,\Sigma_0+\Sigma_1)(\Sigma_0+\Sigma_1)
=\bar\nu_0\Sigma_0+\left.\partial_\Sigma(\bar\nu\Sigma)\right|_0\Sigma_1+O(\Sigma_1^2).
$$

The [viscous transport response exponent](../../../../../../viscous-transport-response-exponent.md) satisfies $\partial_\Sigma(\bar\nu\Sigma)|_0=q\bar\nu_0$. Subtract the background equation and retain only linear terms to obtain

$$
\boxed{\partial_t\Sigma_1=\frac3r\partial_r\left[r^{1/2}\partial_r(r^{1/2}q\bar\nu_0\Sigma_1)\right].}
$$

This remains a [linear equation](../../../../../../linear-equation.md) with space- and time-dependent background coefficients; neither a steady background nor constant $q$ is required for this step. The sign of the response coefficient is the [negative-diffusion criterion for viscous disk instability](../../../../../../negative-diffusion-criterion-for-viscous-disk-instability.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
