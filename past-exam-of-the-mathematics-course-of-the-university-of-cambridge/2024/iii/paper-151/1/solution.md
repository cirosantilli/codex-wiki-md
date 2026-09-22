<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $P_\bullet\to\mathbb Z$ be a [projective resolution](../../../../../projective-resolution.md) of the trivial $\mathbb ZG$-module. The [projective-resolution definition of group cohomology](../../../../../projective-resolution-definition-of-group-cohomology.md) is

$$
H^n(G,M)=H^n\!\left(\operatorname{Hom}_{\mathbb ZG}(P_\bullet,M)\right).
$$

This is independent, up to a natural [isomorphism](../../../../../isomorphism.md), of the chosen [projective resolution](../../../../../projective-resolution.md).

The degreewise natural isomorphisms

$$
\operatorname{Hom}_{\mathbb ZG}(P_j,M_1\oplus M_2)
\cong\operatorname{Hom}_{\mathbb ZG}(P_j,M_1)
\oplus\operatorname{Hom}_{\mathbb ZG}(P_j,M_2)
$$

commute with the [coboundary maps](../../../../../coboundary-map.md). Taking [cohomology](../../../../../cohomology-split.md) proves that [group cohomology commutes with finite direct sums](../../../../../group-cohomology-commutes-with-finite-direct-sums.md):

$$
H^n(G,M_1\oplus M_2)
\cong H^n(G,M_1)\oplus H^n(G,M_2).
$$

Now restrict $P_\bullet$ from $G$ to a subgroup $K$. The [group ring](../../../../../group-ring.md) $\mathbb ZG$ is free as a $\mathbb ZK$-module, so restriction carries [free modules](../../../../../free-module.md) to free modules and [projective modules](../../../../../projective-module.md) to projective modules. Thus the restricted complex is a [projective resolution](../../../../../projective-resolution.md) of the trivial $\mathbb ZK$-module. For the [coinduced module](../../../../../coinduced-module.md) $Y=\operatorname{Hom}_{\mathbb ZK}(\mathbb ZG,X)$, the [Hom functor adjunction for a coinduced module](../../../../../hom-functor-adjunction-for-a-coinduced-module.md) gives an isomorphism of [cochain complexes](../../../../../cochain-complex.md)

$$
\operatorname{Hom}_{\mathbb ZG}(P_\bullet,Y)
\cong\operatorname{Hom}_{\mathbb ZK}(P_\bullet,X).
$$

Explicitly, a map $F$ is sent to $p\mapsto F(p)(1)$; the inverse sends a $\mathbb ZK$-linear map $a$ to $p\mapsto(r\mapsto a(rp))$. Taking [cohomology](../../../../../cohomology-split.md) proves [Shapiro's lemma](../../../../../shapiro-s-lemma.md):

$$
H^n(G,Y)\cong H^n(K,X).
$$

For the [conjugation module of a group ring](../../../../../conjugation-module-of-a-group-ring.md) $N=\mathbb ZG_{\mathrm{conj}}$, the basis $G$ is the disjoint union of its [conjugacy classes](../../../../../conjugacy-class.md). Hence $N$ is the [direct sum](../../../../../direct-sum.md) of the integral permutation modules on those classes. The class of a representative $g_i$ is the transitive $G$-set $G/C_G(g_i)$, where $C_G(g_i)$ is its [centralizer](../../../../../centralizer.md). Since $G$ is finite, this permutation module is both induced and coinduced from the trivial $C_G(g_i)$-module $\mathbb Z$. Applying [group cohomology commutes with finite direct sums](../../../../../group-cohomology-commutes-with-finite-direct-sums.md) and [Shapiro's lemma](../../../../../shapiro-s-lemma.md) yields the [group cohomology of a conjugation module](../../../../../group-cohomology-of-a-conjugation-module.md):

$$
H^n(G,N)\cong\bigoplus_iH^n(C_G(g_i),\mathbb Z).
$$

The [symmetric group](../../../../../symmetric-group.md) $S_3$ has three [conjugacy classes](../../../../../conjugacy-class.md), represented by the identity, a transposition, and a three-cycle. Their [centralizers](../../../../../centralizer.md) are respectively

$$
S_3,\qquad C_2,\qquad C_3.
$$

For any [finite group](../../../../../finite-group.md) $L$ acting trivially on $\mathbb Z$,

$$
H^1(L,\mathbb Z)=\operatorname{Hom}(L,\mathbb Z)=0,
$$

because a [group homomorphism](../../../../../group-homomorphism.md) sends an element of finite order to an element of finite order, while the [additive group](../../../../../additive-group.md) of the integers contains no nonzero [torsion elements](../../../../../torsion-element.md). Therefore

$$
H^1(S_3,N)=0.
$$

The [periodic resolution of a finite cyclic group](../../../../../periodic-resolution-of-a-finite-cyclic-group.md) alternates the maps $t-1$ and $1+t+\cdots+t^{m-1}$. After applying $\operatorname{Hom}_{\mathbb ZC_m}(-,\mathbb Z)$ with the trivial action, these become alternately zero and multiplication by $m$, proving

$$
H^2(C_m,\mathbb Z)\cong\mathbb Z/m\mathbb Z.
$$

Combining this calculation with the supplied $H^2(S_3,\mathbb Z)\cong\mathbb Z/2\mathbb Z$ gives

$$
\boxed{H^2(S_3,N)
\cong\mathbb Z/2\mathbb Z\oplus\mathbb Z/2\mathbb Z\oplus\mathbb Z/3\mathbb Z.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 151](../../paper-151-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
