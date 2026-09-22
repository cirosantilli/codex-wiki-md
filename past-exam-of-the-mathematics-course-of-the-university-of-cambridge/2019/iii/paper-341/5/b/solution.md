<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [mass matrix](../../../../../../mass-matrix.md) is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), and [integration by parts](../../../../../../integration-by-parts.md) with periodic boundary conditions gives $C^T=-C$. Hence

$$
\frac{d}{dt}(U^TMU)=2U^TCU=0.
$$

This is [energy conservation for semidiscrete Galerkin advection](../../../../../../energy-conservation-for-semidiscrete-galerkin-advection.md): $U^TMU=\|u_h\|_{L^2(0,1)}^2$. Thus the semidiscretization is **stable and conserves its finite element [L2 norm](../../../../../../l2-norm.md)**.

For a mesh-independent comparison with the grid norm, the [Fourier symbol](../../../../../../fourier-symbol-of-a-difference-operator.md) of $M$ is $h(2+\cos\theta)/3$, between $h/3$ and $h$. Consequently

$$
\frac h3\sum_m|U_m|^2\leq U^*MU\leq h\sum_m|U_m|^2.
$$

The conserved energy therefore gives a uniform bound in $\sqrt{h\sum_m|U_m|^2}$ as well. Equivalently, each [Fourier mode](../../../../../../fourier-mode.md) evolves with the purely imaginary exponent $\sigma(\theta)=3i\sin\theta/[h(2+\cos\theta)]$. This concerns the semidiscrete method; a chosen time integrator must separately control those imaginary [eigenvalues](../../../../../../eigenvalue.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
