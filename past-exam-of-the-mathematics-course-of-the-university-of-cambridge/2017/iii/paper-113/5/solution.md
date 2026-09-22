<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Put $R_j=S/I_j$ and $R_0=S$. The hypothesis says multiplication by $F_j$ on the graded ring $R_{j-1}$ is injective for $j=2,3$. Checking homogeneous elements suffices: an arbitrary annihilated element splits into homogeneous components, each annihilated separately because $F_j$ and $I_{j-1}$ are homogeneous. Also $F_1\ne0$ because it has degree $d_1>0$, and $S$ is an [integral domain](../../../../../integral-domain.md). Thus $F_1,F_2,F_3$ is a [regular sequence](../../../../../regular-sequence.md), and the suggested [short exact sequences](../../../../../short-exact-sequence.md) become

$$
0\longrightarrow R_{j-1}(-d_j)\xrightarrow{\ \cdot F_j\ }R_{j-1}\longrightarrow R_j\longrightarrow0.
$$

Sheafification and twisting preserve exactness. With $X_0=\mathbb P^4_{\mathbb C}$, the resulting sequences, interpreted on the ambient projective space via the closed inclusions, are

$$
0\longrightarrow\mathcal O_{X_{j-1}}(m-d_j)
\longrightarrow\mathcal O_{X_{j-1}}(m)
\longrightarrow\mathcal O_{X_j}(m)\longrightarrow0.
$$

[Cohomology under a closed immersion](../../../../../cohomology-under-a-closed-immersion.md) identifies the displayed sheaf cohomology with that on $X_j$. For every integer $m$, [cohomology of twisting sheaves on projective space](../../../../../cohomology-of-twisting-sheaves-on-projective-space.md) gives $H^q(X_0,\mathcal O(m))=0$ for $1\le q\le3$. Inducting through the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) gives

$$
H^q(X_j,\mathcal O_{X_j}(m))=0\qquad(1\le q\le3-j).
$$

Indeed the two adjacent groups have degrees $q$ and $q+1$ on $X_{j-1}$, both in its vanishing range. This is [intermediate cohomology vanishing for a projective complete intersection](../../../../../intermediate-cohomology-vanishing-for-a-projective-complete-intersection.md).

We simultaneously prove $H^0(X_j,\mathcal O_{X_j}(m))=0$ for $m<0$ and $H^0(X_j,\mathcal O_{X_j})=\mathbb C$. Both hold on $X_0$ by the same projective-space formula. For $j\le3$, the preceding stage has $H^1(X_{j-1},\mathcal O(m-d_j))=0$. If $m<0$, both degree-zero groups on that stage vanish, so the new one vanishes. If $m=0$, the left degree-zero group vanishes because $-d_j<0$, while the middle group is $\mathbb C$. Therefore the natural restriction of constant functions is an isomorphism at every stage:

$$
\boxed{H^0(X_1,\mathcal O_{X_1})=H^0(X_2,\mathcal O_{X_2})=H^0(X_3,\mathcal O_{X_3})=\mathbb C.}
$$

These are isomorphisms of $\mathbb C$-algebras, not just vector spaces. The [global regular functions on a positive-dimensional projective complete intersection](../../../../../global-regular-functions-on-a-positive-dimensional-projective-complete-intersection.md) are constants even if the complete intersection is singular or nonreduced; smoothness and reducedness were not assumed.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 113](../../paper-113-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
