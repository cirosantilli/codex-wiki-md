<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Time independence of $V$ makes the [Green function](../../../../../green-s-function-split.md) depend on $t,t'$ through $\tau=t-t'$. A spatially varying potential does not imply spatial [translation](../../../../../translation-geometry.md) invariance. Fix $\mathbf r'$ and set $\mathbf x=\mathbf r-\mathbf r'$; write the Fourier coefficient more fully as $G_{\mathbf r'}(\mathbf k;\omega)$. The [source](../../../../../source-quantum-field-theory.md) position is an implicit parameter in the printed notation. Define

$$
V_{\mathbf r'}(\mathbf q)=\int d^3x\,V(\mathbf r'+\mathbf x)e^{-i\mathbf q\cdot\mathbf x}=e^{i\mathbf q\cdot\mathbf r'}\widetilde V(\mathbf q).
$$

The ordinary derivative terms transform into $(-\omega^2+k^2+m^2)G_{\mathbf r'}$. The product $V\partial_tG$ becomes a [convolution](../../../../../convolution.md), and $2ie(-i\omega)=2e\omega$. More explicitly, insert both inverse spatial [Fourier transforms](../../../../../fourier-transform-split.md) into $VG$: the integral over $\mathbf x$ enforces $\mathbf q+\mathbf k'=\mathbf k$. The transformed delta [source](../../../../../source-quantum-field-theory.md) is one, leaving

$$
\boxed{(-\omega^2+k^2+m^2)G_{\mathbf r'}(\mathbf k;\omega)+2e\omega\int\frac{d^3k'}{(2\pi)^3}V_{\mathbf r'}(\mathbf k-\mathbf k')G_{\mathbf r'}(\mathbf k';\omega)=1.}
$$

This is a [source-position-dependent Fourier Green function](../../../../../source-position-dependent-fourier-green-function.md). Dropping the explicit $\mathbf r'$ subscripts recovers the requested notation with exactly the potential transform defined in the source. No assumption of a homogeneous potential is needed. The factor $(2\pi)^{-3}$ and the source-position phase are necessary for the stated Fourier convention.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
