<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We use the equilibrium [generalized Langevin equation](../../../../generalized-langevin-equation.md) and its [generalized fluctuation-dissipation relation](../../../../generalized-fluctuation-dissipation-relation.md), with the factor $5$ in the noise [autocorrelation](../../../../autocorrelation.md) fixing the equilibrium [velocity](../../../../velocity.md) [variance](../../../../variance-split.md). Let $g$ be the [velocity](../../../../velocity.md) relaxation function and let a tilde denote a one-sided [Laplace transform](../../../../laplace-transform.md):

$$
g'(t)=-\int_0^t\kappa(u)g(t-u)\,du,
\qquad g(0)=1,
\qquad
\widetilde g(s)=\frac1{s+\widetilde\kappa(s)}.
$$

The equilibrium [velocity](../../../../velocity.md) [autocorrelation function](../../../../autocorrelation.md) is $\chi(t)=5g(t)$, so

$$
\boxed{\widetilde\chi(s)=\frac5{s+\widetilde\kappa(s)},\qquad \chi(0)=5.}
$$

For completeness, this relation follows without assuming independence of the noise and [velocity](../../../../velocity.md) in a stationary infinite history. The two-sided noise [power spectral density](../../../../power-spectral-density.md) is $S_R(\omega)=10\operatorname{Re}\widetilde\kappa(i\omega)$. The stable linear equation has [velocity](../../../../velocity.md) transfer function $H(i\omega)=[i\omega+\widetilde\kappa(i\omega)]^{-1}$, so

$$
S_V(\omega)=|H(i\omega)|^2S_R(\omega)
=10\operatorname{Re}H(i\omega).
$$

This is precisely the [power spectral density](../../../../power-spectral-density.md) of the even extension of $5g(t)$. Stable relaxation removes initial transients with a finite second [moment](../../../../moment.md), giving the long-time [autocorrelation function](../../../../autocorrelation.md) defined in the question. All the parameter choices used below have stable relaxation.

Integrating the [velocity autocorrelation function](../../../../velocity-autocorrelation-function.md) twice gives the [mean squared displacement](../../../../mean-squared-displacement.md) from a fixed initial [position](../../../../position.md):

$$
\mathbb E\bigl[(X(t)-X(0))^2\bigr]
=2\int_0^t(t-u)\chi(u)\,du.
$$

A decaying initial transient does not change its asymptotic slope. Therefore the [Green-Kubo formula for diffusion](../../../../green-kubo-formula-for-diffusion.md) gives

$$
D=\int_0^\infty\chi(u)\,du
=\widetilde\chi(0)
=\frac5{\widetilde\kappa(0)}.
$$

For the given friction [memory kernel](../../../../memory-kernel.md), direct [integration](../../../../integral-split.md) yields

$$
\widetilde\kappa(s)=\frac{c_1}{s+c_3}+\frac{c_1c_2}{(s+c_3)^2},
\qquad
\widetilde\kappa(0)=\frac{c_1}{c_3}+\frac{c_1c_2}{c_3^2}.
$$

At $c_1=c_2=c_3=1$, the integrated friction is $2$, hence

$$
\boxed{D=\frac52.}
$$

The relaxation denominator here is $s^3+2s^2+2s+2$. Its roots have negative real parts by the cubic [Routh-Hurwitz criterion](../../../../routh-hurwitz-stability-criterion.md), since all coefficients are positive and $2\cdot2>2$. This justifies the decay and [integrability](../../../../integrability.md) used above. The [diffusion coefficient](../../../../diffusion-coefficient.md) depends on the area under the friction [memory kernel](../../../../memory-kernel.md), not just its value at zero.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the stochastic modelling of biological processes course of the University of Oxford](../../../split.md)
5. [Stochastic modelling of biological processes course of the University of Oxford](../../../../stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
