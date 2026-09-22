<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a dimensionless [Hamiltonian](../../../../../../hamiltonian.md) in the functional weight $e^{-H}$, assume $\alpha>0$, and let $\phi(\mathbf x)=\int_{|\mathbf p|\leq\Lambda}d^Dp\,(2\pi)^{-D}e^{i\mathbf p\cdot\mathbf x}\widetilde\phi(\mathbf p)$. Reality means $\widetilde\phi(-\mathbf p)=\widetilde\phi(\mathbf p)^*$. At zero field, the [quadratic form](../../../../../../quadratic-form.md) is

$$
H_0=\frac12\int_{|\mathbf p|\leq\Lambda}\frac{d^Dp}{(2\pi)^D}\left(\alpha^{-1}p^2+r_0\right)|\widetilde\phi(\mathbf p)|^2.
$$

In the [momentum-shell renormalization group](../../../../../../momentum-shell-renormalization-group.md), split into $\phi_<+\phi_>$ below and above $\Lambda/b$. Disjoint Fourier supports make the [quadratic form](../../../../../../quadratic-form.md) split into $H_0[\phi_<]+H_0[\phi_>]$. Integration over the shell gives a source-independent [Gaussian functional integral](../../../../../../gaussian-functional-integral.md) multiplying the [partition function](../../../../../../canonical-partition-function.md), or an additive constant in the effective [free energy](../../../../../../thermodynamic-free-energy.md); it leaves the slow-mode quadratic coefficients unchanged before rescaling. A uniform field has support only at zero momentum, so it does not change this shell integration.

Restore the [ultraviolet cutoff](../../../../../../ultraviolet-cutoff.md) by $\mathbf p'=b\mathbf p$, $\mathbf x'=\mathbf x/b$, and choose

$$
\phi'(\mathbf x')=b^{(D-2)/2}\phi_<(b\mathbf x'),\qquad \widetilde\phi'(\mathbf p')=b^{-(D+2)/2}\widetilde\phi_< (\mathbf p'/b).
$$

The measure, two gradients and two fields have scale factors $b^D$, $b^{-2}$ and $b^{-(D-2)}$, whose product is one. The mass term has factor $b^D b^{-(D-2)}=b^2$, while the uniform source term has factor $b^D b^{-(D-2)/2}=b^{(D+2)/2}$. Hence the [Gaussian momentum-shell scaling](../../../../../../gaussian-momentum-shell-scaling.md) is

$$
\boxed{\alpha^{-1}\longmapsto\alpha^{-1},\qquad r_0\longmapsto b^2r_0,\qquad h\longmapsto b^{(D+2)/2}h.}
$$

For a slowly varying nonuniform source the corresponding formula is $h'(\mathbf x')=b^{(D+2)/2}h(b\mathbf x')$. Here the nonuniform source on the right is its projection onto the retained [Fourier modes](../../../../../../fourier-mode.md); an eliminated source component contributes only to the field-independent Gaussian normalization. The field [engineering dimension](../../../../../../engineering-dimension.md) is $(D-2)/2$ and its Gaussian [anomalous dimension](../../../../../../anomalous-dimension.md) is zero. The mass and uniform source are relevant perturbations of the [Gaussian fixed point](../../../../../../gaussian-fixed-point.md). Positivity of $\alpha$ is necessary for a stable [kinetic term](../../../../../../kinetic-term.md) near this point. One can use a finite volume and positive mass as infrared regulators and then take the critical limit; at exactly zero mass the integral over the zero [Fourier mode](../../../../../../fourier-mode.md) alone is not a normalized finite-volume [Gaussian measure](../../../../../../gaussian-measure.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
