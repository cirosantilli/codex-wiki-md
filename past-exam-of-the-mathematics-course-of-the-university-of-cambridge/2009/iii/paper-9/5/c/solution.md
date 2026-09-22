<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is [Weyl lemma](../../../../../../weyl-lemma.md), with the representative condition needed for pointwise smoothness. Choose a smooth radial nonnegative [mollifier](../../../../../../mollifier.md) $\rho_\varepsilon$ of mass one. On interior domains, $f_\varepsilon=f*\rho_\varepsilon$ is smooth and harmonic because $\Delta f_\varepsilon=(\Delta f)*\rho_\varepsilon=0$.

Fix a smaller interior neighborhood and a radial mollifier $\rho_r$ whose support stays inside the domain there. The [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) implies $f_\varepsilon=f_\varepsilon*\rho_r$ when $\varepsilon$ is sufficiently small: a radial average is a weighted average of spherical means, all equal to the center value.

As $\varepsilon\downarrow0$, $f_\varepsilon\to f$ in $L^1_{\rm loc}$, while $f_\varepsilon*\rho_r\to f*\rho_r$ locally uniformly. The latter follows by bounding the difference by $\|\rho_r\|_\infty$ times the local $L^1$ error on a slightly larger compact set. Thus $f=f*\rho_r$ almost everywhere locally. The right side is smooth, and its Laplacian is zero, providing a smooth harmonic representative. These representatives agree on overlapping neighborhoods since continuous functions agreeing almost everywhere agree everywhere.

The given uniqueness of the canonical upper semicontinuous representative identifies this smooth function with $\widetilde f$. Since the question assumes $f=\widetilde f$, it follows that $\boxed{f\in C^\infty(\Omega)}$ pointwise. An arbitrary null-set modification of a harmonic distribution would not have that conclusion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
