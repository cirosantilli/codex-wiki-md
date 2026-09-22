<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $a=c/(4\pi en)$ and retain terms linear in $\delta\mathbf B$. The [electron magnetohydrodynamics](../../../../../../electron-magnetohydrodynamics.md) induction equation becomes

$$
\partial_t\delta\mathbf B=-aB_0\partial_z(\nabla\times\delta\mathbf B).
$$

Here the [curl](../../../../../../curl.md) of $(\nabla\times\delta\mathbf B)\times B_0\hat{\mathbf z}$ reduces to $B_0\partial_z\nabla\times\delta\mathbf B$, since the background [magnetic field](../../../../../../magnetic-field.md) is constant and the [divergence](../../../../../../divergence.md) of a curl vanishes. For a [plane wave](../../../../../../plane-wave.md) $\delta\mathbf B=\mathbf b\,e^{i(\mathbf k\cdot\mathbf r-\omega t)}$, the linear equation and the [solenoidal](../../../../../../solenoidal-vector-field.md) constraint are

$$
\omega\mathbf b=i aB_0k_\parallel\,\mathbf k\times\mathbf b,\qquad \mathbf k\cdot\mathbf b=0.
$$

On the transverse plane, the operator $i\mathbf k\times$ has [eigenvalues](../../../../../../eigenvalue.md) $\pm k$ by the [helicity decomposition of a transverse Fourier mode](../../../../../../helicity-decomposition-of-a-transverse-fourier-mode.md). Equivalently, squaring the equation and using the [vector triple product](../../../../../../vector-triple-product.md) gives $\omega^2=a^2B_0^2k_\parallel^2k^2$. Since $aB_0=v_Ad_i$, where $v_A$ is the [Alfvén speed](../../../../../../alfven-speed.md) and $d_i$ the [ion skin depth](../../../../../../ion-skin-depth.md),

$$
\boxed{\omega_\pm(\mathbf k)=\pm v_Ad_i k_\parallel k.}
$$

The two branches have opposite [circular polarizations](../../../../../../circular-polarization.md). The specified electron-only induction model describes a [whistler wave](../../../../../../whistler-wave.md); the paper calls these branches [kinetic Alfvén waves](../../../../../../kinetic-alfven-wave.md). The following cascade calculation uses the specified model and its [dispersion relation](../../../../../../dispersion-relation.md), without adding the pressure response needed for the usual kinetic Alfvén interpretation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
