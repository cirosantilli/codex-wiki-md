<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The flat [unitary connection](../../../../../../unitary-connection.md) on $E_V$ is its [Chern connection](../../../../../../chern-connection.md), since it preserves the induced [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) and its $(0,1)$ part is the [Dolbeault operator](../../../../../../dolbeault-operator.md). Its curvature is zero. The trace-curvature formula for the [degree of a holomorphic vector bundle](../../../../../../degree-of-a-holomorphic-vector-bundle.md) therefore gives

$$
\deg E_V=\frac{i}{2\pi}\int_X\operatorname{tr}F_{E_V}=0,
\qquad \mu(E_V)=0.
$$

For any positive-rank proper [holomorphic subbundle](../../../../../../holomorphic-subbundle.md) $F\subset E_V$, equip $F$ with the induced metric and use the block-connection calculation of Question 4(a). Since the ambient curvature vanishes, its [Chern curvature](../../../../../../chern-curvature.md) is

$$
F_F=B^\dagger\wedge B=-b^\dagger b\,dz\wedge d\bar z,
$$

where $B=b\,dz$ is the [second fundamental form of a holomorphic subbundle](../../../../../../second-fundamental-form-of-a-holomorphic-subbundle.md). Consequently

$$
\deg F=-\frac1{2\pi}\int_X i\operatorname{tr}(b^\dagger b)\,dz\wedge d\bar z\le0,
\qquad \mu(F)\le0=\mu(E_V).
$$

The term being integrated is nonnegative, so its sign gives the inequality for every such subbundle, not just for parallel subbundles. By the definition of a [semistable holomorphic vector bundle](../../../../../../semistable-holomorphic-vector-bundle.md),

$$
\boxed{E_V\text{ is semistable and has degree }0.}
$$

If semistability is formulated using coherent subsheaves instead, saturate a subsheaf on the smooth curve. The saturation has the same rank, at least as large a degree, and is a subbundle because a torsion-free sheaf on a smooth curve is locally free. The inequality for the saturated subbundle therefore also bounds the original subsheaf. Finally, equality for a subbundle forces $B=0$, so it is parallel; invariant subspaces of $V$ correspond to these degree-zero parallel subbundles. Semistability is the conclusion required here, rather than stability for every unitary representation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
