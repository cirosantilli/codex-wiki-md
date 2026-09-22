<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\boldsymbol c=(U,V)^T$ and $\Gamma=\begin{pmatrix}\gamma_{11}&\gamma_{12}\\\gamma_{12}&\gamma_{22}\end{pmatrix}$. A well-posed anisotropic [diffusion](../../../../../../../diffusion.md) problem requires $\Gamma$ to be symmetric positive definite: $\gamma_{11}>0$ and $\Delta=\gamma_{11}\gamma_{22}-\gamma_{12}^2>0$. For the [normal mode](../../../../../../../normal-mode.md) in the source the [dispersion relation](../../../../../../../dispersion-relation.md) is

$$
\omega=Uk+Vl+i(\mu-\gamma_{11}k^2-2\gamma_{12}kl-\gamma_{22}l^2).
$$

The [group velocity](../../../../../../../group-velocity.md) vanishes when $\boldsymbol c-2i\Gamma\boldsymbol k=0$. Consequently

$$
\boldsymbol k_0=-\frac i2\Gamma^{-1}\boldsymbol c,\qquad
\omega_0=i\left(\mu-\frac14\boldsymbol c^T\Gamma^{-1}\boldsymbol c\right).
$$

The requested [anisotropic absolute-instability threshold for positive diffusion](../../../../../../../anisotropic-absolute-instability-threshold-for-positive-diffusion.md) is

$$
\boxed{\mu>f(U,V),\qquad
f(U,V)=\frac{\gamma_{22}U^2-2\gamma_{12}UV+\gamma_{11}V^2}{4\Delta}}.
$$

For positive definite [diffusion](../../../../../../../diffusion.md) this is also sufficient: the anisotropic [Gaussian heat kernel](../../../../../../../gaussian-heat-kernel.md) has exponential factor $\exp[\mu t-(\boldsymbol x-\boldsymbol c t)^T\Gamma^{-1}(\boldsymbol x-\boldsymbol c t)/(4t)]$ and a $t^{-1}$ prefactor, so its fixed-position [growth rate](../../../../../../../growth-rate.md) is precisely $\mu-f$.

Let the prescribed speed be $q$ and let $d_{\min}\le d_{\max}$ be the positive [eigenvalues](../../../../../../../eigenvalue.md) of $\Gamma$. The [Rayleigh quotient](../../../../../../../rayleigh-quotient.md) for $\Gamma^{-1}$ gives

$$
\min_{|\boldsymbol c|=q}f=\frac{q^2}{4d_{\max}},\qquad
\max_{|\boldsymbol c|=q}f=\frac{q^2}{4d_{\min}}.
$$

Absence of [absolute hydrodynamic instability](../../../../../../../absolute-hydrodynamic-instability.md) for every direction therefore requires

$$
\boxed{\mu\le\frac{q^2}{4d_{\max}}}.
$$

**This is an upper bound on $\mu$, not a minimum required value.** The source's last sentence reverses this monotonicity: reducing the growth parameter always helps, so there is no finite lower threshold guaranteeing absence. If it had asked for instability in every direction, the corresponding condition would be $\mu>q^2/(4d_{\min})$. Without the positive-definite assumption, negative [diffusion](../../../../../../../diffusion.md) directions make the forward problem ill posed; a singular [diffusion](../../../../../../../diffusion.md) tensor requires a separate transport analysis and does not support the displayed inverse-matrix formula.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
