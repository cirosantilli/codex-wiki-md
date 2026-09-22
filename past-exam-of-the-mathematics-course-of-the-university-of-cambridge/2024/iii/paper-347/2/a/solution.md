<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Steady [mass conservation](../../../../../../mass-conservation.md) with inward-positive [accretion rate](../../../../../../accretion-rate.md) gives

$$
\dot m=-2\pi R\Sigma u_R=\text{constant}.
$$

Write the specific angular momentum as $l=R^2\Omega$. Multiplying the azimuthal equation by $2\pi R$ and using the mass equation shows that the sum of advected and viscous angular-momentum flux is constant:

$$
\dot m,l+2\pi\nu\Sigma R^3\frac{d\Omega}{dR}
=\dot m,l_{\rm in}.
$$

The right-hand side implements the [zero-torque inner boundary condition](../../../../../../zero-torque-inner-boundary-condition.md). For a [Keplerian accretion disk](../../../../../../keplerian-accretion-disk.md), $l\propto R^{1/2}$ and $R^3d\Omega/dR=-(3/2)l$. Therefore

$$
\boxed{
\nu\Sigma
=\frac{\dot m}{3\pi}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right]
},
$$

and

$$
\boxed{
u_R
=-\frac{3\nu}{2R}
\left[1-\left(\frac{R_{\rm in}}R\right)^{1/2}\right]^{-1}
}.
$$

Far outside the inner edge, $\Sigma\simeq\dot m/(3\pi\nu)$ and $u_R\simeq-3\nu/(2R)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
