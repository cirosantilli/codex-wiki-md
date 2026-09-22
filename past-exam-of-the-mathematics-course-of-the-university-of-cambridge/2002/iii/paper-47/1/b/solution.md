<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Subtract the ambient [velocity](../../../../../../velocity.md) and [stress](../../../../../../stress.md), writing $\mathbf u'=\mathbf u-\mathbf u_\infty$. This perturbation decays at infinity and on the [sphere](../../../../../../sphere.md) has [velocity](../../../../../../velocity.md) $\mathbf U+\boldsymbol\Omega\times\mathbf x-\mathbf u_\infty$. The ambient flow is regular through the ball and has no [body force](../../../../../../body-force.md). Its net [torque](../../../../../../torque.md) on the imaginary spherical surface is zero: the [divergence theorem](../../../../../../divergence-theorem.md) converts the [torque](../../../../../../torque.md) to the [volume integral](../../../../../../volume-integral.md) of the [stress](../../../../../../stress.md) [divergence](../../../../../../divergence.md) plus its antisymmetric part, both zero. Thus the perturbation has zero [torque](../../../../../../torque.md) too.

Reciprocity with the auxiliary [rotlet](../../../../../../rotlet.md) gives

$$
\boldsymbol\Omega\cdot\mathbf G=\int_{r=a}\mathbf u_\infty\cdot\boldsymbol\sigma_G\mathbf n_D\,dS.
$$

Using $\boldsymbol\sigma_G\mathbf n_D=3(\mathbf G\times\mathbf x)/(8\pi a^4)$ yields

$$
\boldsymbol\Omega=\frac3{8\pi a^4}\int_{r=a}\mathbf x\times\mathbf u_\infty\,dS.
$$

On this [sphere](../../../../../../sphere.md) $\mathbf x=a\mathbf n$, so the [vector](../../../../../../vector.md) [divergence theorem](../../../../../../divergence-theorem.md) gives $\int\mathbf x\times\mathbf u_\infty dS=a\int_{r<a}\nabla\times\mathbf u_\infty dV$. Taking the [curl](../../../../../../curl.md) of the homogeneous [Stokes equation](../../../../../../stokes-equation.md) makes $\boldsymbol\omega_\infty$ [harmonic](../../../../../../harmonic-function.md). Its ball average is its central value: the derivative of each spherical mean is proportional to the [volume integral](../../../../../../volume-integral.md) of its [Laplacian](../../../../../../laplacian.md), hence zero, and its small-radius limit is its value at the center. Therefore

$$
\boxed{\boldsymbol\Omega=\frac3{8\pi a^3}\frac{4\pi a^3}{3}\boldsymbol\omega_\infty(0)=\frac12\boldsymbol\omega_\infty(0).}
$$

This proves [Faxén rotation law](../../../../../../faxen-s-rotational-law.md) directly from the reciprocal theorem, including why no finite-radius [Laplacian](../../../../../../laplacian.md) correction is needed for a body-force-free ambient flow. Regularity of the ambient field throughout the [sphere](../../../../../../sphere.md)'s prospective interior is part of this argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
