<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

TODO: user-deferred biological kinetic mechanism and its biochemical pattern-forming applications. The remainder treats generic two-field reaction-diffusion physics only.

Let $\mathbf u=(u,v)$ obey $\partial_t\mathbf u=\mathbf f(\mathbf u)+\operatorname{diag}(D_u,D_v)\nabla^2\mathbf u$. At a uniform steady state, write its reaction Jacobian as $J=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$. Without [diffusion](../../../../../diffusion.md) stability requires $a+d<0$ and $\Delta=ad-bc>0$. A Fourier perturbation evolves under $J-q^2\operatorname{diag}(D_u,D_v)$, whose [determinant](../../../../../determinant.md) is

$$
\Delta(q)=\Delta-(D_va+D_ud)q^2+D_uD_vq^4.
$$

Its [trace](../../../../../matrix-trace.md) becomes more negative with increasing $q$. A stationary diffusion-driven instability therefore requires

$$
\boxed{D_va+D_ud>0,\qquad (D_va+D_ud)^2>4D_uD_v\Delta,}
$$

with an allowed domain mode in the resulting negative-determinant band. Equal [diffusivities](../../../../../diffusion-coefficient.md) cannot satisfy this while $a+d<0$. The physical mechanism is that transport can destabilize coupled fields even when the local kinetics relaxes a spatially uniform perturbation. Faster [diffusion](../../../../../diffusion.md) of an inhibitory response is one possible realization.

The selected [wave numbers](../../../../../wavenumber.md) depend on growth rates and boundaries; nonlinear saturation determines the final stripes, spots or other states. Linear instability alone neither supplies a biochemical mechanism nor uniquely predicts a final finite-amplitude pattern.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the soft matter and biological physics course of the University of Cambridge](../../../../split.md)
6. [Soft Matter and Biological Physics course of the University of Cambridge](../../../../../soft-matter-and-biological-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
