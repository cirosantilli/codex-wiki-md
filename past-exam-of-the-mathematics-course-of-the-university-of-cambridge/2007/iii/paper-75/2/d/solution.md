<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Linearization](../../../../../../linearization.md) removes the [Poisson bracket](../../../../../../poisson-bracket.md) from $\nabla_\parallel$. For Fourier perturbations proportional to $e^{i\mathbf k\cdot\mathbf x-i\omega t}$, the two reduced equations become

$$
-i\omega\Psi=iv_A^2d_ik_\parallel b,\qquad-i\omega b=id_ik_\parallel k_\perp^2\Psi.
$$

Eliminating either amplitude gives

$$
\boxed{\omega^2=v_A^2d_i^2k_\parallel^2k_\perp^2,\qquad\omega=\pm k_\parallel v_Ad_ik_\perp.}
$$

Since $k=(k_\perp^2+k_\parallel^2)^{1/2}=k_\perp[1+O(\epsilon^2)]$, this is the specified [dispersion relation](../../../../../../dispersion-relation.md) to the accuracy of the anisotropic reduction. The reduced equations cannot retain the subleading correction replacing $k_\perp$ by the full $k$.

The full [electron magnetohydrodynamics](../../../../../../electron-magnetohydrodynamics.md) equation checks that correction directly. Its [linearization](../../../../../../linearization.md) is $\partial_t\delta\mathbf B=-\alpha B_0\partial_z\nabla\times\delta\mathbf B$. Hence

$$
-i\omega\delta\mathbf B=\alpha B_0k_\parallel\mathbf k\times\delta\mathbf B.
$$

Applying the cross-product operator twice and using $\mathbf k\cdot\delta\mathbf B=0$ gives

$$
\boxed{\omega^2=(\alpha B_0)^2k_\parallel^2k^2=v_A^2d_i^2k_\parallel^2k^2.}
$$

Thus the full model gives the stated relation exactly and the reduced model gives its leading anisotropic limit, with all signs and normalization factors consistent.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
