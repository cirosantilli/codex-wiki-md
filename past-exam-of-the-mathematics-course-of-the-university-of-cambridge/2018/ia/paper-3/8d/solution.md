<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

The [internal direct product theorem](../../../../../internal-direct-product-theorem.md) states that if $H,K\trianglelefteq G$, $H\cap K=\{1\}$, and $HK=G$, then $G\cong H\times K$. Indeed, for $h\in H,k\in K$, the commutator $[h,k]$ lies in both $H$ and $K$, so it is trivial. The map $(h,k)\mapsto hk$ is consequently a homomorphism; the intersection condition makes it injective and $HK=G$ makes it surjective. Conversely, the two factors in a direct product satisfy these conditions.

In odd dimension, $-I$ is central and has determinant $-1$. Every $Q\in O(3)$ has a unique expression $Q=(-I)^\varepsilon R$ with $R\in SO(3)$, so

$$
\boxed{O(3)\cong SO(3)\times C_2.}
$$

By contrast, $SO(2)\times C_2$ is abelian, while reflections in $O(2)$ conjugate a rotation to its inverse. Thus **$O(2)\not\cong SO(2)\times C_2$**.

The center of the [unitary group](../../../../../unitary-group.md) consists exactly of scalar unitary matrices:

$$
\boxed{Z(U(2))=\{zI:|z|=1\}.}
$$

The determinant gives a surjective homomorphism

$$
\det:U(2)\longrightarrow\mathbb T
$$

whose kernel is the [special unitary group](../../../../../special-unitary-group.md) $SU(2)$.

Nevertheless $U(2)$ is not isomorphic to $SU(2)\times\mathbb T$. The center of $U(2)$ has exactly one nonidentity element of order two, namely $-I$. The center of the proposed product is $\{\pm I\}\times\mathbb T$, which has three nonidentity elements of order two. Since an isomorphism preserves the center and element orders,

$$
\boxed{U(2)\not\cong SU(2)\times\mathbb T.}
$$

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
