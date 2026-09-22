<h1 id="6d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For either coefficient system $\mathbb Z$ or $\mathbb F_p$, multiplying two matrices keeps all entries in that system, and multiplicativity of the [determinant](../../../../../../determinant.md) preserves [determinant](../../../../../../determinant.md) one. The identity matrix has [determinant](../../../../../../determinant.md) one, and for a determinant-one matrix the [matrix inverse](../../../../../../matrix-inverse.md) is

$$
\begin{pmatrix}a&b\\c&d\end{pmatrix}^{-1}
=\begin{pmatrix}d&-b\\-c&a\end{pmatrix}.
$$

Its entries again belong to the same coefficient system and its [determinant](../../../../../../determinant.md) is one. Together with associativity of [matrix multiplication](../../../../../../matrix-multiplication.md), these facts establish all the [group axioms](../../../../../../group-axioms.md). Thus both sets are [special linear groups](../../../../../../special-linear-group.md).

Reduce each entry modulo five to define

$$
\pi:SL_2(\mathbb Z)\longrightarrow SL_2(\mathbb F_5),\qquad M\longmapsto\overline M.
$$

Reduction respects sums and products, so $\overline{MN}=\overline M\,\overline N$. It also respects the [determinant](../../../../../../determinant.md), ensuring that the image has [determinant](../../../../../../determinant.md) one. Hence $\pi$ is a [group homomorphism](../../../../../../group-homomorphism.md). Its [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) consists exactly of determinant-one integer matrices congruent to the identity modulo five:

$$
\boxed{\ker\pi=\left\{\begin{pmatrix}1+5a&5b\\5c&1+5d\end{pmatrix}\in SL_2(\mathbb Z):a,b,c,d\in\mathbb Z\right\}.}
$$

The determinant-one condition remains part of this set; the four integers cannot be chosen independently without it. A [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) is a [normal subgroup](../../../../../../normal-subgroup.md), since $\pi(gkg^{-1})=\pi(g)e\pi(g)^{-1}=e$ for $k\in\ker\pi$. This is the [principal congruence subgroup](../../../../../../principal-congruence-subgroup.md) of level five.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
