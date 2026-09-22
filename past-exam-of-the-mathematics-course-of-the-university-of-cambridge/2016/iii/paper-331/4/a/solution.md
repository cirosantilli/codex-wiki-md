<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [kinetic-energy inner product](../../../../../../kinetic-energy-inner-product.md) $\langle v,u\rangle=\int v^*\cdot u\,dV$, with perturbation energy $\|u\|^2/2$. On divergence-free fields the primal generator, before the pressure projection, is

$$
A(t)u=-(\boldsymbol U\cdot\nabla)u-(u\cdot\nabla)\boldsymbol U+\mathrm{Re}^{-1}\nabla^2u.
$$

The base state is also divergence-free. The periodic boundary terms in $x,z$ cancel, and decay at $|y|\to\infty$ removes the remaining boundary terms. [Integration by parts](../../../../../../integration-by-parts.md) changes $-\boldsymbol U\cdot\nabla$ to $+\boldsymbol U\cdot\nabla$; the [Laplacian](../../../../../../laplacian.md) is self-adjoint under these conditions. Writing $J_{ij}=\partial_jU_i$, the shear term $-Ju$ has [adjoint operator](../../../../../../adjoint-operator.md) $-J^Tv$. A [pressure gradient](../../../../../../pressure-gradient.md) pairs to zero with a divergence-free field. Hence

$$
A^\dagger(t)v=(\boldsymbol U\cdot\nabla)v-(\nabla\boldsymbol U)^Tv+\mathrm{Re}^{-1}\nabla^2v-\nabla\pi,
$$

where the last term enforces the divergence-free projection.

To conserve $\langle v(t),u_p(t)\rangle$ over the finite interval, the physical-time adjoint obeys $-\partial_tv=A^\dagger(t)v$. Put $\tau=-t$ and $u_d(\tau)=v(-\tau)$; then $\partial_\tau u_d=A^\dagger(-\tau)u_d$. This reverses the interval from $t=T$ towards $t=0$, or $\tau=-T$ towards $\tau=0$.

For $\boldsymbol\Omega=\nabla\times\boldsymbol U$, the [vorticity cross-product identity](../../../../../../vorticity-cross-product-identity.md) and the [curl of a cross product](../../../../../../curl-of-a-cross-product.md)

$$
\boldsymbol\Omega\times u_d=(u_d\cdot\nabla)\boldsymbol U-(\nabla\boldsymbol U)^Tu_d,\qquad
\nabla\times(\boldsymbol U\times u_d)=(u_d\cdot\nabla)\boldsymbol U-(\boldsymbol U\cdot\nabla)u_d
$$

hold when both fields are divergence-free. Their difference equals the transport and shear terms in the [adjoint operator](../../../../../../adjoint-operator.md). Therefore **the adjoint linearized Navier-Stokes evolution is**

$$
\boxed{\partial_\tau\boldsymbol u_d=\boldsymbol\Omega(-\tau)\times\boldsymbol u_d-
\nabla\times[\boldsymbol U(-\tau)\times\boldsymbol u_d]-\nabla p_d+\mathrm{Re}^{-1}\nabla^2\boldsymbol u_d,\qquad
\nabla\cdot\boldsymbol u_d=0.}
$$

The [Leray-Helmholtz projection](../../../../../../leray-helmholtz-projection.md) determines the adjoint pressure. The time-dependent base state is evaluated at $-\tau$; no extra time derivative of that base state appears in the spatial [adjoint operator](../../../../../../adjoint-operator.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
