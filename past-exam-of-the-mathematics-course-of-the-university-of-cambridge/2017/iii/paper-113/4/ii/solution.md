<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $U_0=D_+(t_0)=\operatorname{Spec}\mathbb C[x]$, where $x=t_1/t_0$, and $U_1=D_+(t_1)=\operatorname{Spec}\mathbb C[y]$, with $y=1/x$ on the overlap. Since $\mathcal G$ is a [quasi-coherent sheaf](../../../../../../quasi-coherent-sheaf.md), it is associated to a $\mathbb C[x]$-module $M$ on $U_0$. The preimages under the open inclusion $f$ of $U_0,U_1,U_0\cap U_1$ are $U_0,D(x),D(x)$, all [affine schemes](../../../../../../affine-scheme.md). Thus $f$ is an [affine morphism](../../../../../../affine-morphism.md) and its [direct image sheaf](../../../../../../direct-image-sheaf.md) $f_*\mathcal G$ is quasi-coherent by [direct image of a quasi-coherent sheaf under an affine morphism](../../../../../../direct-image-of-a-quasi-coherent-sheaf-under-an-affine-morphism.md).

The two-chart cover is an [acyclic cover](../../../../../../acyclic-cover.md) by [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md), so the [acyclic cover theorem](../../../../../../leray-s-theorem.md) identifies its [Čech cohomology](../../../../../../cech-cohomology.md) with [sheaf cohomology](../../../../../../sheaf-cohomology.md). Its only potentially nontrivial positive-degree differential is

$$
M\oplus M_x\longrightarrow M_x,\qquad (m,n)\longmapsto n-m/1.
$$

This is surjective because of the second summand. There are no normalized Čech terms in degree two or higher for a two-open cover, so

$$
\boxed{H^i(\mathbb P^1_{\mathbb C},f_*\mathcal G)=0\qquad(i>0).}
$$

This is the [acyclic direct image from an affine chart of the projective line](../../../../../../acyclic-direct-image-from-an-affine-chart-of-the-projective-line.md). The pushforward need not itself be a flasque sheaf; the acyclic affine cover is what justifies this computation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
