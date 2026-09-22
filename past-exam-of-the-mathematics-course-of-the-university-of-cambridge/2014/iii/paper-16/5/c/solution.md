<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Marsden-Weinstein theorem](../../../../../../marsden-weinstein-theorem.md) says that for a [Hamiltonian group action](../../../../../../hamiltonian-group-action.md), if $c$ is a [regular value](../../../../../../regular-value.md) fixed by the [coadjoint action](../../../../../../coadjoint-representation.md) and $G$ acts freely and properly on $\mu^{-1}(c)$, then

$$
M_c=\mu^{-1}(c)/G
$$

is a [symplectic manifold](../../../../../../symplectic-manifold.md) with a unique form characterized by $\pi^*\omega_c=\iota^*\omega$, where $\iota$ includes the level set and $\pi$ is the quotient projection. Its dimension is $\dim M-2\dim G$.

Equip $\mathbb C^{n+1}$ with the [standard symplectic form](../../../../../../standard-symplectic-form.md)

$$
\omega_{\mathbb C}=\sum_{j=0}^n dx_j\wedge dy_j=\frac i2\sum_{j=0}^n dz_j\wedge d\bar z_j.
$$

Let the [circle group](../../../../../../circle-group.md) act by $e^{i\theta}\cdot z=e^{i\theta}z$. Its generator is $X=\sum_j(-y_j\partial_{x_j}+x_j\partial_{y_j})$, and

$$
\iota_X\omega_{\mathbb C}=-d\left(\frac12|z|^2\right).
$$

Consequently the [moment map](../../../../../../moment-map.md) in our convention is $\mu(z)=-|z|^2/2$. It is invariant, hence equivariant because the [circle group](../../../../../../circle-group.md) is abelian. The level $\mu^{-1}(-1)$ is the sphere of radius $\sqrt2$; it is regular, the [circle group](../../../../../../circle-group.md) acts freely there, and properness follows from compactness of the group. The quotient is [Complex projective space](../../../../../../complex-projective-space.md), by $z\mapsto[z]$, a scaled [Hopf fibration](../../../../../../hopf-fibration.md). The [Marsden-Weinstein theorem](../../../../../../marsden-weinstein-theorem.md) therefore produces a reduced [symplectic form](../../../../../../symplectic-form.md) on $\mathbb{CP}^n$.

To identify it rather than only assert its existence, use the primitive

$$
\lambda_0=\frac12\sum_j(x_jdy_j-y_jdx_j)
=\frac1{4i}\sum_j(\bar z_jdz_j-z_jd\bar z_j),\qquad d\lambda_0=\omega_{\mathbb C}.
$$

On the affine chart choose the local section $s(w)=\sqrt2(1,w)/\sqrt S$ of the quotient. Direct substitution gives

$$
s^*\lambda_0=\frac1{2iS}\sum_j(\bar w_jdw_j-w_jd\bar w_j)
=\frac1{2i}(\partial-\bar\partial)\log S.
$$

Differentiating, using $\bar\partial\partial=-\partial\bar\partial$, gives

$$
\boxed{\omega_c=s^*\omega_{\mathbb C}=d(s^*\lambda_0)=i\partial\bar\partial\log S=\omega_{\mathrm{FS}}.}
$$

This is the [Fubini-Study form from circle reduction](../../../../../../fubini-study-form-from-circle-reduction.md). The unit sphere instead produces half this form; our radius $\sqrt2$ is exactly what gives the $2\pi$ line-area normalization used above.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
