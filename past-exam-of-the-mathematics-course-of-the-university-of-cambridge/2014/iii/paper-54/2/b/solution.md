<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [continuity equation](../../../../../../continuity-equation.md) and integrate by parts, with the stated vanishing boundary terms and finite moments. The [second mass moment tensor](../../../../../../second-mass-moment-tensor.md) satisfies

$$
\dot I_{ij}=\int\rho(u_ix_j+x_iu_j)\,d\tau,
$$

and differentiation again gives

$$
\ddot I_{ij}=2\int\rho u_iu_j\,d\tau+\int\rho(x_iD_tu_j+x_jD_tu_i)\,d\tau.
$$

Insert the stress-[divergence](../../../../../../divergence.md) equation from part (a). The two force integrals become

$$
\int(x_i\partial_kT_{jk}+x_j\partial_kT_{ik})\,d\tau=-\int(T_{ji}+T_{ij})\,d\tau=-2\mathcal T_{ij}.
$$

The first term is $4K_{ij}$. Hence the [magnetized-fluid tensor virial theorem](../../../../../../magnetized-fluid-tensor-virial-theorem.md) is

$$
\boxed{\frac12\ddot I_{ij}=2K_{ij}-\mathcal T_{ij}.}
$$

Here $\mathcal T$ is the volume-integrated stress, whose sign differs from some gravitational potential-energy tensor conventions. The derivation also requires the advective mass-moment surface terms to vanish; this is automatic for an isolated sufficiently decaying configuration.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
