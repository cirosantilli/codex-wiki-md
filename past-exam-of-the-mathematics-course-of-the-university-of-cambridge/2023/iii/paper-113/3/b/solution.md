<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a finite affine cover $\mathcal U=(U_j)$ of the [Noetherian scheme](../../../../../../noetherian-scheme.md) $X$. Because $X$ is [separated](../../../../../../separated-scheme.md), every finite intersection $U_J$ is affine. Its inverse image $V_J=Z\cap U_J$ under the [closed immersion](../../../../../../closed-immersion.md) is also affine. By the definition of the [direct image sheaf](../../../../../../direct-image-sheaf.md),

$$
(i_*\mathcal F)(U_J)=\mathcal F(V_J).
$$

The [Čech complexes](../../../../../../cech-cochain-complex.md) for $i_*\mathcal F$ on $\mathcal U$ and for $\mathcal F$ on the induced cover $(Z\cap U_j)$ are therefore identical, including their restriction maps. Both affine covers are acyclic for the relevant [quasi-coherent sheaves](../../../../../../quasi-coherent-sheaf.md), so the [acyclic cover theorem](../../../../../../leray-s-theorem.md) gives

$$
H^q(X,i_*\mathcal F)\cong H^q(Z,\mathcal F)
$$

for every $q$. This is [cohomology under a closed immersion](../../../../../../cohomology-under-a-closed-immersion.md).

For $X=\mathbb P_k^n$, use its $n+1$ standard affine opens. The induced cover of $Z$ is still acyclic, and its Čech complex has no cochains in degrees greater than $n$. The [cohomological dimension bound from an affine cover](../../../../../../cohomological-dimension-bound-from-an-affine-cover.md) therefore yields

$$
\boxed{H^q(Z,\mathcal F)=0\qquad(q>n).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
