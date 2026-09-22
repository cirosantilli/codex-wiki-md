<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the photon phase-space coordinates $(\mathbf x,q,\mathbf n)$, with $q=ap$ and $\mathbf n$ its propagation direction. Divide the [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md) by $d\tau/d\lambda$ and apply the chain rule. The homogeneous blackbody distribution is time independent at fixed comoving momentum because its physical temperature scales as $a^{-1}$. Therefore

$$
\partial_\tau f_1+\frac{dx^i}{d\tau}\partial_i f_1+q'\frac{df_0}{dq}+q'\partial_qf_1+(n^i)'\partial_{n^i}f_1=0.
$$

On the unperturbed ray $dx^i/d\tau=n^i$; its correction is first order and multiplies the first-order spatial gradient of $f_1$. Similarly $q'$ and $(n^i)'$ are first order, so their products with derivatives of $f_1$ are second order. The zeroth-order distribution has no directional dependence. Keeping only linear terms and using $q'=-qh'_{ij}n^in^j/2$ gives

$$
\partial_\tau f_1+n^i\partial_i f_1=\frac12qf_0'(q)h'_{ij}n^in^j.
$$

After Fourier transforming with $e^{i\mathbf k\cdot\mathbf x}$ and $\mu=\widehat{\mathbf k}\cdot\mathbf n$, the [Free-streaming photon Boltzmann equation](../../../../../../free-streaming-photon-boltzmann-equation.md) in synchronous variables is

$$
\boxed{f_1'+ik\mu f_1=\frac12qf_0'(q)h'_{ij}n^in^j.}
$$

Direction deflection is a real first-order geodesic effect, but its effect on the already perturbed distribution starts at second order here.

Let $I_0=\int_0^\infty q^3f_0(q)dq$, so in the phase-space normalization being used $a^4\bar\rho_\gamma=4\pi I_0$. The [photon brightness perturbation](../../../../../../photon-brightness-perturbation.md) is $\Delta=I_0^{-1}\int q^3f_1dq$. This agrees with the stated density normalization, and $I_0$ is independent of [conformal time](../../../../../../conformal-time.md). Integrating the distribution equation gives

$$
\Delta'+ik\mu\Delta=\frac{h'_{ij}n^in^j}{2I_0}\int_0^\infty q^4f_0'(q)dq.
$$

For a [Planck distribution](../../../../../../planck-photon-distribution.md), the endpoint term $[q^4f_0]_0^\infty$ vanishes. Integration by parts yields $\int q^4f_0' dq=-4I_0$. Thus the [synchronous photon brightness equation](../../../../../../synchronous-photon-brightness-equation.md) is

$$
\boxed{\Delta'+ik\mu\Delta=-2h'_{ij}n^in^j.}
$$

For a small directional blackbody temperature shift $\Theta=\Delta T/T$, expansion gives $f_1=-qf_0'(q)\Theta$. The same integral then gives $\Delta=4\Theta$, also following from blackbody energy density proportional to $T^4$. This temperature interpretation presumes a perturbed blackbody shape; frequency-integrated brightness can still be defined for more general distributions.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
