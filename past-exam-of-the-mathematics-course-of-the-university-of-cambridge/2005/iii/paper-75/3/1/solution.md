<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Interpret the multiplicative [Gaussian white noise](../../../../../../gaussian-white-noise.md) as the limit of a smooth short-correlation-time velocity field, hence in the [Stratonovich integral](../../../../../../stratonovich-integral.md) convention. Put $\partial_i=\partial/\partial B_i$. For a realization, differentiating the field-space [Dirac delta](../../../../../../dirac-delta-function.md) gives its field-space [continuity equation](../../../../../../continuity-equation.md)

$$
\partial_t\widetilde P=-\partial_i(\sigma_{im}B_m\widetilde P).
$$

The velocity-gradient covariance has zero trace variance: contracting $T_{mn}^{ij}$ with $m=i,n=j$ gives $3-(9+3)/4=0$. Thus the gradient is trace free, consistently with the incompressible ideal induction equation.

A noise impulse in component $\sigma_{jn}$ changes $\widetilde B_j$ by $\widetilde B_n$ times that impulse. Its instantaneous retarded action on the [Dirac delta](../../../../../../dirac-delta-function.md) is therefore

$$
\frac{\delta\widetilde P}{\delta\sigma_{jn}}=-\partial_j(B_n\widetilde P).
$$

Only earlier times affect the present field. In the white-noise limit the integral over this causal interval has $\int_0^t\delta(t-t')\,dt'=1/2$, corresponding to the symmetric short-time regularization. Applying the [Furutsu–Novikov formula](../../../../../../novikov-s-theorem.md) and then averaging gives

$$
\langle\sigma_{im}\widetilde P\rangle=-\frac{\kappa_2}{2}T_{mn}^{ij}\partial_j(B_nP).
$$

Substitute into the averaged field-space [continuity equation](../../../../../../continuity-equation.md):

$$
\partial_tP=\frac{\kappa_2}{2}\partial_i\left[B_mT_{mn}^{ij}\partial_j(B_nP)\right].
$$

The differentiated $B_n$ term vanishes because $\sum_jT_{mj}^{ij}=0$, and the remaining contraction is

$$
T_{mn}^{ij}B_mB_n=B^2\delta_{ij}-\frac12B_iB_j.
$$

Consequently the closed vector [Fokker-Planck equation](../../../../../../fokker-planck-equation.md) for [Gaussian white-noise magnetic stretching](../../../../../../gaussian-white-noise-magnetic-stretching.md) is

$$
\boxed{\partial_tP=\frac{\kappa_2}{2}\partial_i\left[\left(B^2\delta_{ij}-\frac12B_iB_j\right)\partial_jP\right].}
$$

This is a positive [diffusion](../../../../../../diffusion.md) operator: the displayed matrix has eigenvalues $B^2$ on the two transverse directions and $B^2/2$ along $\mathbf B$. Replacing the endpoint half-weight by one would double the [diffusion](../../../../../../diffusion.md) and fail to reproduce the later rate.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
