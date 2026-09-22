<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $G_1=\phi(\mathbf r|\mathbf r_1)$ and $G_2=\phi(\mathbf r|\mathbf r_2)$. [Green's second identity](../../../../../../green-second-identity.md) gives

$$
\int_\Omega[G_1(\Delta+k_0^2)G_2-G_2(\Delta+k_0^2)G_1],dV
=\int_S(G_1\partial_nG_2-G_2\partial_nG_1),dS.
$$

The common [Robin boundary condition](../../../../../../robin-boundary-condition.md) makes the surface integrand vanish. Where $\beta\neq0$, substitute $\partial_nG_i=-\alpha G_i/\beta$; a Dirichlet portion also contributes zero. The delta sources therefore give the [Helmholtz Green-function reciprocity](../../../../../../helmholtz-green-function-reciprocity.md)

$$
\boxed{\phi(\mathbf r_1|\mathbf r_2)=\phi(\mathbf r_2|\mathbf r_1).}
$$

This is a bilinear identity, with no complex conjugation. Assume the boundary-value problem has a unique Green kernel; in an exterior problem use the same outgoing radiation condition for both kernels.

For the weighted operator, assume smooth positive $f$ and set $\mathbf b=\nabla\log f$. Then

$$
L=\frac1f\nabla\cdot(f\nabla)+k_0^2=\Delta+\mathbf b\cdot\nabla+k_0^2.
$$

Its unweighted transpose, obtained by [integration by parts](../../../../../../integration-by-parts.md), is

$$
L^{\mathrm T}u=\Delta u-\nabla\cdot(\mathbf bu)+k_0^2u
=\nabla\cdot[f\nabla(u/f)]+k_0^2u.
$$

The associated boundary identity is

$$
\int_\Omega(uLv-vL^{\mathrm T}u),dV
=\int_S[u\partial_nv-v\partial_nu+(\partial_n\log f)uv],dS.
$$

To cancel it when $v$ satisfies the given Robin condition, the required adjoint kernel satisfies

$$
\boxed{\nabla\cdot\left[f\nabla\left(\frac{\widetilde\psi}{f}\right)\right]+k_0^2\widetilde\psi
=\delta(\mathbf r-\mathbf r_2),}
$$



$$
\boxed{\alpha\widetilde\psi+\beta\left(\partial_n\widetilde\psi-\widetilde\psi\,\partial_n\log f\right)=0.}
$$

Using these two delta sources in the boundary identity proves $\psi(\mathbf r_2|\mathbf r_1)=\widetilde\psi(\mathbf r_1|\mathbf r_2)$, the [adjoint reciprocity for a weighted Helmholtz operator](../../../../../../adjoint-reciprocity-for-a-weighted-helmholtz-operator.md). As a check, $L^{\mathrm T}(fv)=fLv$, so

$$
\widetilde\psi(\mathbf r|\mathbf r_2)=\frac{f(\mathbf r)}{f(\mathbf r_2)}\psi(\mathbf r|\mathbf r_2).
$$

This is equivalent to [weighted acoustic Green-function reciprocity](../../../../../../weighted-acoustic-green-function-reciprocity.md), $f(\mathbf r_2)\psi(\mathbf r_2|\mathbf r_1)=f(\mathbf r_1)\psi(\mathbf r_1|\mathbf r_2)$. Unit delta normalization is essential here. A Hermitian adjoint would instead conjugate coefficients and change the radiation convention; the requested equality uses the transpose.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
