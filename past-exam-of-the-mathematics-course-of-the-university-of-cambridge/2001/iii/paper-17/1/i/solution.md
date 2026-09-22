<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the [adjunction](../../../../../../adjoint-functors.md) as the [natural bijection](../../../../../../natural-bijection.md)

$$
\Phi_{A,B}:\mathcal D(FA,B)\longrightarrow\mathcal C(A,GB).
$$

The [unit of an adjunction](../../../../../../unit-of-an-adjunction.md) and [counit of an adjunction](../../../../../../counit-of-an-adjunction.md) are the [natural transformations](../../../../../../natural-transformation.md) whose components are

$$
\boxed{\eta_A=\Phi_{A,FA}(1_{FA}),\qquad
\varepsilon_B=\Phi^{-1}_{GB,B}(1_{GB}).}
$$

[Naturality](../../../../../../naturality.md) of the [hom-set](../../../../../../hom-set.md) bijections gives, for $f:FA\to B$ and $g:A\to GB$,

$$
\Phi_{A,B}(f)=G(f)\eta_A,\qquad
\Phi^{-1}_{A,B}(g)=\varepsilon_B F(g).
$$

For example, postcomposition by $f$ in the first [hom-set](../../../../../../hom-set.md) corresponds to postcomposition by $Gf$ in the second, giving the first formula; naturality in $A$ gives the second. The same [naturality](../../../../../../naturality.md) says that, for $a:A\to A'$ and $b:B\to B'$,

$$
GF(a)\eta_A=\eta_{A'}a,\qquad b\varepsilon_B=\varepsilon_{B'}FG(b).
$$

Thus these components do define the asserted [natural transformations](../../../../../../natural-transformation.md) $1_{\mathcal C}\to GF$ and $FG\to1_{\mathcal D}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
