<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here being modular of weight $k$ means obeying the weight transformation law, or equivalently being invariant under the [slash operator for modular forms](../../../../../../slash-operator-for-modular-forms.md):

$$
f\!\left(\frac{a\tau+b}{c\tau+d}\right)=(c\tau+d)^kf(\tau)\qquad\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma.
$$

This transformation property alone does not impose holomorphy; a holomorphic [modular form](../../../../../../modular-form.md) additionally satisfies interior and cusp holomorphy. That distinction is needed for the nonholomorphic completion in the next part.

Put $F(\tau)=f(N\tau)$. For $\gamma\in\Gamma_0(N)$, conjugation by $\operatorname{diag}(N,1)$ gives the integral determinant-one [matrix](../../../../../../matrix.md)

$$
\gamma_N=\begin{pmatrix}a&Nb\\c/N&d\end{pmatrix}\in SL_2(\mathbb Z),\qquad N\gamma\tau=\gamma_N(N\tau).
$$

Since the denominator in the latter action is $(c/N)(N\tau)+d=c\tau+d$, the full-group modularity of $f$ gives

$$
\boxed{F(\gamma\tau)=(c\tau+d)^kF(\tau)\qquad\gamma\in\Gamma_0(N).}
$$

Thus argument dilation lowers the group to the [Gamma 0 congruence subgroup](../../../../../../gamma-0-congruence-subgroup.md) while retaining the weight. If $f$ is a holomorphic [modular form](../../../../../../modular-form.md), cusp holomorphy is preserved too: an integral [matrix](../../../../../../matrix.md) $\operatorname{diag}(N,1)\gamma$ of determinant $N$ factors as an integral determinant-one [matrix](../../../../../../matrix.md) times an upper triangular positive-determinant [matrix](../../../../../../matrix.md). The corresponding slash translate is a constant times $f((a\tau+b)/d)$ with positive $a/d$, whose expansion at infinity has no negative exponents. This checks every rational cusp; for a [cusp form](../../../../../../cusp-form.md) its constant term remains zero. It is the level-one instance of the [degeneracy map for cusp forms](../../../../../../degeneracy-map-for-cusp-forms.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
