<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $u_i=\langle v_i\rangle$ and use summation over repeated Cartesian indices. A mass-normalized [galactic distribution function](../../../../../../galactic-distribution-function.md) obeys the [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md)

$$
\partial_tf+v_i\partial_{x_i}f-(\partial_{x_i}\phi)\partial_{v_i}f=0.
$$

Assume $f$ decays in [velocity](../../../../../../velocity.md) sufficiently fast that the necessary boundary terms vanish. Its zeroth velocity moment gives the [continuity equation](../../../../../../continuity-equation.md)

$$
\partial_t\rho+\partial_{x_i}(\rho u_i)=0.
$$

For the first velocity moment, multiply by $v_j$ and integrate. In the gravitational term, [integration by parts](../../../../../../integration-by-parts.md) gives $\int v_j\partial_{v_i}f\,d^3v=-\delta_{ij}\rho$. Therefore

$$
\partial_t(\rho u_j)+\partial_{x_i}\bigl(\rho\langle v_iv_j\rangle\bigr)=-\rho\partial_{x_j}\phi.
$$

The [velocity-dispersion tensor](../../../../../../velocity-dispersion-tensor-of-collisionless-matter.md) is the centered second moment, so $\langle v_iv_j\rangle=u_iu_j+\sigma_{ij}^2$. Expanding the streaming terms, the factor multiplying $u_j$ cancels by the [continuity equation](../../../../../../continuity-equation.md):

$$
\partial_t(\rho u_j)+\partial_{x_i}(\rho u_iu_j)
=\rho\partial_tu_j+\rho u_i\partial_{x_i}u_j.
$$

Hence the [Jeans equation](../../../../../../jeans-equation.md) is

$$
\boxed{\rho\bigl(\partial_tu_j+u_i\partial_{x_i}u_j\bigr)
=-\rho\partial_{x_j}\phi-\partial_{x_i}(\rho\sigma_{ij}^2).}
$$

Its fluid analogue is the momentum equation with pressure tensor $P_{ij}=\rho\sigma_{ij}^2$. For isotropic random motion, $P_{ij}=P\delta_{ij}$, and this becomes the [Euler equations for an inviscid fluid](../../../../../../euler-equations-for-an-inviscid-fluid.md):

$$
\boxed{\rho\left(\partial_t\boldsymbol u+(\boldsymbol u\cdot\nabla)\boldsymbol u\right)
=-\rho\nabla\phi-\nabla P.}
$$

The tensor form allows anisotropic stellar stresses. In a fluid an [equation of state](../../../../../../equation-of-state.md) can provide a pressure closure; the [Jeans equation](../../../../../../jeans-equation.md) alone does not determine the [velocity-dispersion tensor](../../../../../../velocity-dispersion-tensor-of-collisionless-matter.md) of a [collisionless stellar system](../../../../../../collisionless-stellar-system.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
