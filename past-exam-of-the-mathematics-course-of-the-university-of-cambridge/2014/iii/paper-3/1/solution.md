<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write a finite [quiver](../../../../../quiver.md) as $Q=(Q_0,Q_1,s,t)$, with vertex and arrow sets and source/target maps. A [representation of a quiver](../../../../../representation-of-a-quiver.md) assigns a [vector space](../../../../../vector-space-split.md) $X_i$ to each vertex and a [linear map](../../../../../linear-map.md) $f_\rho:X_{s(\rho)}\to X_{t(\rho)}$ to each arrow. A [quiver representation morphism](../../../../../quiver-representation-morphism.md) $h:X\to Y$ is a family satisfying $h_{t(\rho)}f_\rho=g_\rho h_{s(\rho)}$.

The [path algebra](../../../../../path-algebra.md) $A=kQ$ has every directed path, including each length-zero path $e_i$, as a [basis](../../../../../basis.md). Multiplication is composition when endpoints match, and zero otherwise; in $pq$, the path $q$ is traversed first. The [orthogonal idempotents](../../../../../orthogonal-idempotent.md) satisfy $1=\sum_ie_i$.

The [path-algebra module equivalence](../../../../../path-algebra-module-equivalence.md) is explicit. From a representation, form $M=\bigoplus_iX_i$, let $e_i$ project onto $X_i$, and let each path act by the composite of its arrow maps. Conversely, an $A$-[module](../../../../../module-mathematics.md) gives $X_i=e_iM$ and $f_\rho(x)=\rho x$. An $A$-[module homomorphism](../../../../../module-homomorphism.md) restricts to the required vertex maps, and a compatible family extends by direct sum. These constructions are mutually inverse up to their evident natural identifications.

**$kQ$ is finite-dimensional exactly when $Q$ is finite and has no oriented cycle.** For a finite [acyclic quiver](../../../../../acyclic-quiver.md), paths have length at most $|Q_0|-1$. An oriented cycle has arbitrarily many distinct powers, giving infinitely many basis paths. If arbitrary infinite quivers are allowed, finiteness of both vertices and arrows is also necessary; the unital module correspondence above uses finite $Q_0$.

Choose only the orientation $1\to2\to3$. The [interval representations of an equioriented three-vertex quiver](../../../../../interval-representations-of-an-equioriented-three-vertex-quiver.md) $I[a,b]$ have $k$ at vertices $a,\ldots,b$, zero elsewhere, and identity arrows within that interval. The complete list is

$$
\boxed{I[1,1],\ I[2,2],\ I[3,3],\ I[1,2],\ I[2,3],\ I[1,3]}.
$$

Here is an elementary proof, without the [Gabriel theorem](../../../../../gabriel-s-theorem.md). For $X_1\xrightarrow fX_2\xrightarrow gX_3$, set $K=\operatorname{im}f\cap\ker g$. Choose $F$ complementing $K$ in $\operatorname{im}f$, $G$ complementing $K$ in $\ker g$, and $H$ complementing $\operatorname{im}f+\ker g$ in $X_2$. Then $X_2=K\oplus F\oplus G\oplus H$, and $g$ is injective on $F\oplus H$. Lift bases of $K,F$ to a complement of $\ker f$ in $X_1$, and extend the bases of $gF,gH$ to $X_3$. These bases split $X$ into precisely the six kinds of interval block. Every block has [endomorphism ring](../../../../../endomorphism-ring.md) $k$, hence is indecomposable, and their different supports make them pairwise nonisomorphic. The same basis argument handles arbitrary vertex dimensions; each indecomposable block itself is finite-dimensional.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
