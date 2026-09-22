<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\tau=x+iy\in\mathfrak h$. For

$$
\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma(1),
$$

the imaginary part of the [Möbius transformation](../../../../../../mobius-transformation.md) is

$$
\operatorname{Im}(\gamma\tau)=\frac{y}{|c\tau+d|^2}.
$$

Among the primitive integer pairs $(c,d)$, choose one minimizing the nonzero quantity $|c\tau+d|$. Such a minimum exists because only finitely many [lattice points](../../../../../../lattice-point.md) lie in a bounded region. Complete $(c,d)$ to a matrix $\gamma\in SL_2(\mathbb Z)$. Then $\gamma\tau$ has maximal imaginary part in its [modular group](../../../../../../modular-group.md) orbit.

Applying an integral translation does not change that imaginary part, so arrange

$$
-\frac12\leq\operatorname{Re}(\gamma\tau)\leq\frac12.
$$

If $\operatorname{Im}(\gamma\tau)<\sqrt3/2$, then $|\gamma\tau|<1$. The modular inversion $S:z\mapsto-1/z$ would give

$$
\operatorname{Im}(S\gamma\tau)
=\frac{\operatorname{Im}(\gamma\tau)}{|\gamma\tau|^2}
>\operatorname{Im}(\gamma\tau),
$$

contradicting maximality. Hence every orbit meets the stated region. This is the [reduction to the standard modular region](../../../../../../reduction-to-the-standard-modular-region.md) argument.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
