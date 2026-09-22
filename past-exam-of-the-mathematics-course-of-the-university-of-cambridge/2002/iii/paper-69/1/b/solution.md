<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) convention

$$
h(\mathbf x)=\int_{\mathbf q}h_{\mathbf q}e^{i\mathbf q\cdot\mathbf x},\qquad
\int_{\mathbf q}=\int\frac{d^Dq}{(2\pi)^D},\qquad h_{-\mathbf q}=h_{\mathbf q}^*.
$$

[Parseval's identity](../../../../../../parseval-identity.md) and $\nabla\mapsto i\mathbf q$ give the diagonal quadratic form

$$
\boxed{\beta H_2=\frac{\beta\sigma}{2}\int_{\mathbf q}q^2h_{\mathbf q}h_{-\mathbf q}.}
$$

In a finite periodic box one can equivalently use orthonormal discrete [Fourier modes](../../../../../../fourier-mode.md), for which each independent real amplitude has a positive stiffness $\sigma q^2$. Fourier orthogonality eliminates all cross terms between different modes. The zero mode is removed as explained in part (a).

The stiffness vanishes as $q\to0$, so [capillary waves](../../../../../../capillary-wave.md) at long wavelength have arbitrarily low energy. The [statistical Hamiltonian](../../../../../../statistical-hamiltonian.md) is invariant under $h(\mathbf x)\mapsto h(\mathbf x)+a$ for any constant $a$. Selecting a particular mean membrane height breaks this continuous normal-translation [symmetry](../../../../../../symmetry-physics.md). A varying local translation therefore has a [gradient](../../../../../../gradient.md) cost but no restoring mass: these are [Goldstone modes](../../../../../../goldstone-boson.md). The diagonal static kernel is $q^2$; it should not be identified with a dynamical frequency without specifying the surrounding fluid or membrane inertia.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
