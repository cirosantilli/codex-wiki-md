<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The density has the form

$$
\rho=C r^{p-2}\Psi^{2p+1},
\qquad
\beta=1-\frac p2.
$$

Insert the ansatz $\sigma_r^2=k\Psi$ into the [Spherical Jeans equation](../../../../../../spherical-jeans-equation.md)

$$
\frac{d(\rho\sigma_r^2)}{dr}
+\frac{2\beta}{r}\rho\sigma_r^2
=\rho\frac{d\Psi}{dr}.
$$

The radial-power derivative cancels the anisotropy term because $p-2+2\beta=0$, leaving $k(2p+2)=1$. Thus

$$
\boxed{
\sigma_r^2=\frac{\Psi}{2(p+1)},
\qquad
\sigma_\theta^2=\sigma_\phi^2
=\frac{p\Psi}{4(p+1)}}.
$$

Their sum is independent of $p$:

$$
\langle v^2\rangle
=\sigma_r^2+\sigma_\theta^2+\sigma_\phi^2
=\frac\Psi2=-\frac\Phi2.
$$

Therefore the local kinetic-energy density and gravitational potential-energy density are

$$
K=\frac12\rho\langle v^2\rangle=-\frac14\rho\Phi,
\qquad
W=\frac12\rho\Phi,
$$

and they satisfy the [local virial relation of the hypervirial model](../../../../../../local-virial-relation-of-the-hypervirial-model.md)

$$
\boxed{2K+W=0}
$$

at every radius. This pointwise identity is not generic. The ordinary [virial theorem](../../../../../../virial-theorem.md) constrains suitable global integrals, with boundary terms when the system is truncated, but does not normally impose a virial balance shell by shell.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
