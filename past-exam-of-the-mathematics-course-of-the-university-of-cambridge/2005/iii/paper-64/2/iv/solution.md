<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Double contraction of the projected [Gauss equation](../../../../../../gauss-equation.md), with the timelike-normal sign and curvature convention in the question, gives

$$
R^{(3)}=q^{\mu\rho}q^{\nu\sigma}R^{(4)}_{\mu\nu\rho\sigma}-K^2+K_{\mu\nu}K^{\mu\nu}.
$$

Here $q^{\mu\nu}=g^{\mu\nu}+n^\mu n^\nu$. Expanding the two projectors gives

$$
q^{\mu\rho}q^{\nu\sigma}R^{(4)}_{\mu\nu\rho\sigma}
=R^{(4)}+2R^{(4)}_{\mu\nu}n^\mu n^\nu.
$$

The four-normal contraction vanishes by Riemann antisymmetry. Because $g_{\mu\nu}n^\mu n^\nu=-1$, the right side is $2G^{(4)}_{\mu\nu}n^\mu n^\nu$. Rearranging proves the [Hamiltonian constraint](../../../../../../hamiltonian-constraint.md) identity:

$$
\boxed{G^{(4)}_{\mu\nu}n^\mu n^\nu=\frac12\left[R^{(3)}+K^2-K_{\mu\nu}K^{\mu\nu}\right].}
$$

For flat FRW, $R^{(3)}=0$, $K^2=9H^2$ and $K_{\mu\nu}K^{\mu\nu}=3H^2$, so $G_{nn}=3H^2$. Einstein's equation is therefore the first [Friedmann equation](../../../../../../friedmann-equations.md), $3H^2=8\pi G\rho$, or $3H^2=8\pi G\rho+\Lambda$ if a cosmological constant is placed separately in Einstein's equation.

The scalar $R^{(3)}$ measures intrinsic spatial curvature, $K^2$ measures squared volume expansion, and the norm of $K_{ij}$ measures directional expansion including shear. More generally $K_{ij}=Kq_{ij}/3+s_{ij}$ with trace-free $s_{ij}$ gives $K_{ij}K^{ij}=K^2/3+s_{ij}s^{ij}$. The shear vanishes in FRW, leaving the positive $3H^2$ contribution. This is an instantaneous constraint on initial data, not the separate acceleration equation.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
