<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define $K=Z_+-Z_-$. Its antisymmetric off-diagonal entries cancel, leaving

$$
\boxed{K=\frac{2\rho\omega}{D}\operatorname{diag}(p,s),\qquad K^{-1}=\frac{D}{2\rho\omega}\operatorname{diag}(1/p,1/s).}
$$

From $\mathbf v=\mathbf v^++\mathbf v^-$ and $\mathbf t=-Z_+\mathbf v^+-Z_-\mathbf v^-$, solve explicitly for the [P-SV characteristic reconstruction](../../../../../../p-sv-characteristic-reconstruction.md):

$$
\boxed{\mathbf v^+=-K^{-1}(\mathbf t+Z_-\mathbf v),\qquad\mathbf v^-=K^{-1}(\mathbf t+Z_+\mathbf v).}
$$

The prescribed strictly positive $p,s$ make this decomposition unique; a grazing or [evanescent](../../../../../../evanescent-wave.md) branch is outside these assumptions.

In the mean flux, the two mixed directional terms are

$$
\frac12\operatorname{Re}\left[(\mathbf v^-)^\dagger Z_+\mathbf v^++(\mathbf v^+)^\dagger Z_-\mathbf v^-\right]=0,
$$

because $Z_-=-Z_+^\dagger$ makes the second scalar minus the [complex conjugate](../../../../../../complex-conjugate.md) of the first. The remaining self terms give

$$
\boxed{\langle S_z\rangle=\frac{\rho\omega}{2D}\left[p\left(|v_x^+|^2-|v_x^-|^2\right)+s\left(|v_z^+|^2-|v_z^-|^2\right)\right].}
$$

Finally use either directional velocity-potential [matrix](../../../../../../matrix.md). Its weighted quadratic form satisfies

$$
p|v_x^\pm|^2+s|v_z^\pm|^2=\omega^2D\left(p|\phi_\pm|^2+s|\psi_\pm|^2\right).
$$

Indeed the two P-SV cross terms have coefficients $-kps$ and $+kps$ for the forward field, with the signs reversed for the backward field, so they cancel. Substitution proves

$$
\boxed{\langle S_z\rangle=\frac{\rho\omega^3}{2}\left[p\left(|\phi_+|^2-|\phi_-|^2\right)+s\left(|\psi_+|^2-|\psi_-|^2\right)\right].}
$$

Thus net normal [elastic-wave energy flux](../../../../../../elastic-wave-energy-flux.md) is the difference of the independently flux-weighted P and SV directional powers, even for coherent mixtures.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
