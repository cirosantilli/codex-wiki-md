<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\widehat{\mathcal O}=[\mathcal O(S)^{\mathrm{op}},\mathbf{Set}]$, with [categorical presheaf](../../../../../../presheaf-category-theory.md) restrictions $X(U)\to X(V)$ when $V\subseteq U$. The five [functors](../../../../../../functor.md) are

$$
\Pi X=X(\varnothing),\qquad \Gamma X=X(S),\qquad
(\Delta A)(U)=A,
$$



$$
(\Lambda A)(U)=
\begin{cases}A&U=\varnothing,\\\varnothing&U\ne\varnothing,\end{cases}
\qquad
(\nabla A)(U)=
\begin{cases}A&U=S,\\\{*\}&U\ne S.\end{cases}
$$

In $\Delta A$ all restriction maps are identities. In $\Lambda A$ and $\nabla A$, all nonidentity restrictions are the unique maps permitted by the displayed [sets](../../../../../../set-split.md). These definitions are valid also when $A$ is empty: a restriction out of $(\nabla A)(S)$ still has singleton target. Maps of [sets](../../../../../../set-split.md) act at the displayed $A$-components, and [natural transformations](../../../../../../natural-transformation.md) act on $\Pi$ and $\Gamma$ by evaluation.

A [natural transformation](../../../../../../natural-transformation.md) $\Lambda A\to X$ is determined by an arbitrary map $A\to X(\varnothing)$, since all other source components are empty. A [natural transformation](../../../../../../natural-transformation.md) $X\to\Delta A$ is determined by its empty-open component $X(\varnothing)\to A$: the component at $U$ must first restrict $X(U)\to X(\varnothing)$. Similarly, a [natural transformation](../../../../../../natural-transformation.md) $\Delta A\to X$ is determined by $A\to X(S)$, followed by the restriction $X(S)\to X(U)$. Finally, a [natural transformation](../../../../../../natural-transformation.md) $X\to\nabla A$ is determined by $X(S)\to A$, since all proper-open targets are singletons. These descriptions give the [hom-set](../../../../../../hom-set.md) bijections

$$
\widehat{\mathcal O}(\Lambda A,X)\cong\mathbf{Set}(A,\Pi X),\qquad
\mathbf{Set}(\Pi X,A)\cong\widehat{\mathcal O}(X,\Delta A),
$$



$$
\widehat{\mathcal O}(\Delta A,X)\cong\mathbf{Set}(A,\Gamma X),\qquad
\mathbf{Set}(\Gamma X,A)\cong\widehat{\mathcal O}(X,\nabla A).
$$

Thus the [five adjoints for constant presheaves on open sets](../../../../../../five-adjoints-for-constant-presheaves-on-open-sets.md) are

$$
\boxed{\Lambda\dashv\Pi\dashv\Delta\dashv\Gamma\dashv\nabla.}
$$

The values at the empty open set are genuine [presheaf](../../../../../../presheaf-of-sets-on-a-topological-space.md) values here; no [sheaf](../../../../../../sheaf-mathematics.md) condition or sheafification is being imposed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
