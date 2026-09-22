<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret the longitudinal [Dirac delta function](../../../../../../dirac-delta-function.md) as the [Markov approximation for a random medium](../../../../../../markov-approximation-for-a-random-medium.md). The two arguments on the left of the printed covariance must be $x_1$ and $x_2$. The transverse [covariance kernel](../../../../../../covariance-kernel.md) is $B(|\mathbf z_1-\mathbf z_2|)$. Here [statistical isotropy](../../../../../../statistical-isotropy.md) means transverse isotropy: a medium with a distinguished longitudinal [white noise](../../../../../../white-noise.md) direction and a smooth transverse covariance is not literally isotropic in all three directions. Also, ideal [Gaussian white noise](../../../../../../gaussian-white-noise.md) replaces the original finite-[variance](../../../../../../variance-split.md) field; it cannot simultaneously satisfy a pointwise normalization $\mathbb E W^2=1$.

Write $Q(r)=\mu^2B(r)$ for the covariance strength of the [refractive index](../../../../../../refractive-index.md) fluctuations. Define the transverse [power spectrum](../../../../../../power-spectrum.md) using the unnormalized forward [Fourier transform](../../../../../../fourier-transform.md) printed in equation 3:

$$
S_F(\boldsymbol\nu)=\int_{\mathbb R^2}Q(|\mathbf r|)e^{-i\boldsymbol\nu\cdot\mathbf r}\,d\mathbf r,\qquad
Q(\mathbf r)=\frac1{(2\pi)^2}\int_{\mathbb R^2}S_F(\boldsymbol\nu)e^{i\boldsymbol\nu\cdot\mathbf r}\,d\boldsymbol\nu.
$$

This is the spectrum of the fluctuations, excluding the deterministic mean index. Equivalently it is the zero-longitudinal-frequency slice of the three-dimensional fluctuation spectrum before the [Markov approximation](../../../../../../markov-approximation-for-a-random-medium.md). The angular integral is $2\pi J_0(\nu r)$, where $J_0$ is the [Bessel function of the first kind](../../../../../../bessel-function-of-the-first-kind.md). Consequently [Fourier inversion](../../../../../../fourier-inversion-theorem.md) and the [Hankel transform](../../../../../../hankel-transform.md) give

$$
S_F(\nu)=2\pi\int_0^\infty Q(r)J_0(\nu r)r\,dr,\qquad
Q(r)=\frac1{2\pi}\int_0^\infty S_F(\nu)J_0(\nu r)\nu\,d\nu.
$$

The printed equations 4 and 5 omit these reciprocal factors, and the left-hand side of equation 5 should depend on $r$. They are instead a consistent order-zero [Hankel transform](../../../../../../hankel-transform.md) pair if their $F$ denotes $S_H=S_F/(2\pi)$.

Using $J_0(0)=1$, the mean-field solution in the [Fourier transform](../../../../../../fourier-transform.md) convention is

$$
\boxed{m(x,\mathbf z)=\exp\left[-\frac{k_0^2x}{4\pi}\int_0^\infty S_F(\nu)\nu\,d\nu\right](U_xE_0)(\mathbf z).}
$$

Here $U_x$ is the [Fresnel propagator](../../../../../../fresnel-propagator.md). Finiteness of the integral ensures a finite screen [wave phase](../../../../../../phase-waves.md) [variance](../../../../../../variance-split.md). If the quoted [power spectrum](../../../../../../power-spectrum.md) uses the self-reciprocal [Hankel transform](../../../../../../hankel-transform.md) convention, the same result reads

$$
\boxed{m(x,\mathbf z)=\exp\left[-\frac{k_0^2x}{2}\int_0^\infty S_H(\nu)\nu\,d\nu\right](U_xE_0)(\mathbf z).}
$$

These formulas describe identical media when $S_F=2\pi S_H$; assigning the same numerical function to both spectral conventions describes different covariance strengths.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
