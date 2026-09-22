<h1 id="38a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [five-point Laplacian](../../../../../../five-point-laplacian.md) applied to $f$ has expansion

$$
\Gamma_5f=h^2\Delta f+\frac{h^4}{12}(f_{xxxx}+f_{yyyy})+O(h^6).
$$

The corrected right side $h^2f+(h^2/12)\Gamma_5f$ cancels the $h^4\Delta f/12$ term in $\Gamma_9u$. Consequently

$$
\boxed{h^{-2}\left(\Gamma_9u-h^2f-\frac{h^2}{12}\Gamma_5f\right)=O(h^4).}
$$

More precisely, the unscaled residual's $h^6$ coefficient is $-(u_{xxxxxx}+u_{yyyyyy})/240+(u_{xxxxyy}+u_{xxyyyy})/144$. This [fourth-order correction of the nine-point Poisson stencil](../../../../../../fourth-order-correction-of-the-nine-point-poisson-stencil.md) does not require $f$ to be harmonic.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [38A](../../38a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
