<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $X$ is a [Noetherian scheme](../../../../../../noetherian-scheme.md), choose a finite affine cover $X=\bigcup_iU_i$. Every intersection $U_i\cap U_j$ is quasi-compact, so choose a finite affine cover $U_i\cap U_j=\bigcup_kU_{ijk}$. If $j_i:U_i\hookrightarrow X$ and $j_{ijk}:U_{ijk}\hookrightarrow X$ are the inclusions, the sheaf axiom gives an exact sequence

$$
0\longrightarrow\mathcal F
\longrightarrow\bigoplus_i(j_i)_*(\mathcal F|_{U_i})
\longrightarrow\bigoplus_{i,j,k}(j_{ijk})_*(\mathcal F|_{U_{ijk}}),
$$

where the last arrow is the difference of the two restrictions to each overlap chart.

Applying the left-exact [direct image sheaf](../../../../../../direct-image-sheaf.md) functor identifies $f_*\mathcal F$ with the kernel of

$$
\bigoplus_i(fj_i)_*(\mathcal F|_{U_i})
\longrightarrow
\bigoplus_{i,j,k}(fj_{ijk})_*(\mathcal F|_{U_{ijk}}).
$$

Every map $U_i\to Y$ and $U_{ijk}\to Y$ is a morphism between [affine schemes](../../../../../../affine-scheme.md). Part (a) shows that all sheaves in the two finite sums are [quasi-coherent sheaves](../../../../../../quasi-coherent-sheaf.md). Kernels of morphisms of quasi-coherent sheaves on the affine scheme $Y$ are quasi-coherent, because they correspond to kernels of module homomorphisms. Therefore $f_*\mathcal F$ is quasi-coherent. This is the [quasi-coherence of direct image under a quasi-compact quasi-separated morphism](../../../../../../quasi-coherence-of-direct-image-under-a-quasi-compact-quasi-separated-morphism.md) in the present Noetherian case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
