<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $0<r_1<r_2$, so the shell excludes the possible singularity at the origin. The [divergence and curl of a radial vector field](../../../../divergence-and-curl-of-a-radial-vector-field.md) formula in [spherical coordinates](../../../../spherical-coordinate-system.md) gives

$$
\nabla\cdot\mathbf F
=\frac1{r^2}\frac{d}{dr}\left(r^2r^{-\beta}\right)
=(2-\beta)r^{-\beta-1}.
$$

With [volume element](../../../../volume-element.md) $dV=r^2\sin\theta\,dr\,d\theta\,d\phi$, direct integration gives

$$
\begin{aligned}
\iiint_V\nabla\cdot\mathbf F\,dV
&=\int_{r_1}^{r_2}\int_0^\pi\int_0^{2\pi}
(2-\beta)r^{1-\beta}\sin\theta\,d\phi\,d\theta\,dr\\
&=\boxed{4\pi\left(r_2^{2-\beta}-r_1^{2-\beta}\right).}
\end{aligned}
$$

For the independent boundary calculation, the outer [sphere](../../../../sphere.md) has outward [unit normal vector](../../../../unit-normal.md) $+\hat{\mathbf r}$ and the inner [sphere](../../../../sphere.md) has outward [unit normal vector](../../../../unit-normal.md) $-\hat{\mathbf r}$. Their [fluxes](../../../../flux.md) are

$$
\Phi_{\rm outer}=4\pi r_2^2r_2^{-\beta},\qquad
\Phi_{\rm inner}=-4\pi r_1^2r_1^{-\beta}.
$$

Their sum equals the direct [volume integral](../../../../volume-integral.md), verifying the [divergence theorem](../../../../divergence-theorem.md). The restriction $\beta\ne2$ permits the displayed power-antiderivative step. At $\beta=2$, treated separately, both the shell [volume integral](../../../../volume-integral.md) and net boundary [flux](../../../../flux.md) are zero; the excluded origin must still not be filled in.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
