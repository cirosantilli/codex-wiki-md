<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By part (a), work first with an affine base and its homogeneous equations. Put $S=k[y_0,\ldots,y_n]$, write $S_N$ for its finite-dimensional degree-$N$ [vector space](../../../../../../vector-space-split.md), and use $S_j=0$ for $j<0$. At each base point define the [graded multiplication map for a projective fiber](../../../../../../graded-multiplication-map-for-a-projective-fiber.md)

$$
\mu_N(x):\bigoplus_{i=1}^r S_{N-d_i}\longrightarrow S_N,\qquad (g_i)_i\longmapsto\sum_i g_i f_i(x,y).
$$

Its image is exactly $(I_x)_N$, since taking the degree-$N$ part of any expression in the [homogeneous ideal](../../../../../../homogeneous-ideal.md) discards all other degrees. Moreover

$$
\mathfrak m^N\subseteq I_x\iff(I_x)_N=S_N\iff\mu_N(x)\text{ is surjective},
$$

because degree-$N$ [monomials](../../../../../../monomial.md) generate $\mathfrak m^N$.

Choose [monomial bases](../../../../../../monomial-basis.md) for the domain summands and codomain. Every entry of the resulting [matrix](../../../../../../matrix.md) is a coefficient of one of the $f_i$, hence a [regular function](../../../../../../regular-function.md) of $x$. If $h_N=\dim S_N$, failure of surjectivity is the vanishing of all $h_N$-by-$h_N$ [matrix minors](../../../../../../minor-linear-algebra.md). It is therefore a closed rank-defect locus $C_N$. If the [matrix](../../../../../../matrix.md) has fewer than $h_N$ columns, the failure is automatic and $C_N=X$, also closed. Constants and $N=0$ are covered by the same construction.

Part (c) gives $\pi(Y)=\bigcap_{N\ge0}C_N$, an intersection of closed subsets, hence closed. Apply part (a) to pass back to arbitrary $X$. Thus **projection from $X\times\mathbb P^n$ sends every closed subset to a closed subset**. This proves the [closedness of projection from projective space](../../../../../../closedness-of-projection-from-projective-space.md) without assuming the properness result being proved.

The field convention matters: a [rational-point projection need not be Zariski closed](../../../../../../rational-point-projection-need-not-be-zariski-closed.md). Over $\mathbb R$, the closed equation $y_0^2=t y_1^2$ in $\mathbb A^1\times\mathbb P^1$ has real-point image $[0,\infty)$. Indeed $y_1=0$ would force $y_0=0$, so a solution exists precisely when $t$ is a square in $\mathbb R$. This infinite proper subset of the affine line is not [Zariski closed](../../../../../../zariski-closed-set.md). The valid arbitrary-field theorem uses scheme or geometric images, for which the matrix argument remains valid at every residue field.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
