<h1 id="22f/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The implication is true in every dimension despite the failure of part (iii). The hypothesis gives $\mathcal Ff\in L^2$, since its weight is at least one. Let $g$ be its inverse Fourier-Plancherel transform; then $g\in H^s$ by construction.

Use the [Gaussian approximate identity](../../../../../../gaussian-approximate-identity.md) $G_\varepsilon(x)=\varepsilon^{-n}e^{-\pi|x|^2/\varepsilon^2}$. Its [Fourier transform](../../../../../../fourier-transform.md) is $e^{-\pi\varepsilon^2|\xi|^2}$. [Fourier inversion](../../../../../../fourier-inversion-theorem.md) of this integrable multiplier times the bounded transform of $f$, justified by Fubini, gives the same function both as $G_\varepsilon*f$ and as $G_\varepsilon*g$. The first converges to $f$ in $L^1$, while the second converges to $g$ in $L^2$ by Plancherel and dominated convergence. Along a common sequence, select subsequences converging [almost everywhere](../../../../../../almost-everywhere.md) for both norms. Their limits agree, giving $f=g$ [almost everywhere](../../../../../../almost-everywhere.md). Consequently

$$
\boxed{f\in H^s(\mathbb R^n),\qquad\widehat f=\mathcal Ff\text{ almost everywhere}.}
$$

This proves the requested conclusion without relying on the incorrect general-dimensional kernel assertion.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [22F](../../22f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
