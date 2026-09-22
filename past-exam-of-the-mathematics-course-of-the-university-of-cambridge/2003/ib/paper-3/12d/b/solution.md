<h1 id="12d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A mode has dimensionless damping ratio $k/\alpha_n$, and characteristic roots

$$
s_\pm=-k\pm\sqrt{k^2-\alpha_n^2}.
$$

If $k/\alpha_n\ll1$, the [normal mode](../../../../../../normal-mode.md) oscillates at $\omega_n=\alpha_n+O(k^2/\alpha_n)$ with exponentially decaying envelope $e^{-kt}$. As $k\to0$, the solution approaches the undamped [wave equation](../../../../../../wave-equation-split.md) response.

If $k/\alpha_n\gg1$, the roots are real and negative, with

$$
s_+=-\frac{\alpha_n^2}{2k}+O(\alpha_n^4/k^3),\qquad s_-=-2k+\frac{\alpha_n^2}{2k}+O(\alpha_n^4/k^3).
$$

The mode has a fast transient and a slow nonoscillatory relaxation. After the fast transient, neglecting $y_{tt}$ gives the [diffusion equation](../../../../../../diffusion-equation-split.md) $y_t\simeq c^2y_{xx}/(2k)$ for these long-wavelength modes. At $k=\alpha_n$, the repeated root produces $te^{-kt}$: this is [critical damping](../../../../../../critical-damping.md).

Thus **the critical parameter is $k/\alpha_n=1$ for each mode**, and the fundamental threshold is

$$
\boxed{\frac{kl}{\pi c}=1.}
$$

When $k<\pi c/l$ every mode is oscillatory. For any fixed, finite $k$, sufficiently large $n$ still gives oscillatory modes, so large damping of the lowest modes does not mean that every mode of the full string is overdamped.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12D](../../12d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
