<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [idele group](../../../../../../idele-group.md) is the [restricted product](../../../../../../restricted-product.md)

$$
J_K=\prod_v'K_v^*,
$$

with respect to $\mathcal O_v^*$ at the finite places. Thus $a=(a_v)$ is an [idele](../../../../../../idele.md) if all components are nonzero and $a_v$ is a unit at all but finitely many finite places. Its topology has basic open sets which equal the full unit subgroup outside finitely many places; it is not just the subspace topology of the unrestricted product. The group is locally compact, and the diagonal $K^*$ consists of the [principal ideles](../../../../../../principal-idele.md). The [idèle class group](../../../../../../idele-class-group.md) is $C_K=J_K/K^*$.

The finite [valuations](../../../../../../valuation.md) give the [idele-to-ideal homomorphism](../../../../../../idele-to-ideal-homomorphism.md)

$$
(a_v)\longmapsto\prod_{v<\infty}\mathfrak p_v^{v(a_v)}.
$$

Its kernel is the product of the finite unit groups and the infinite multiplicative groups; [principal ideles](../../../../../../principal-idele.md) map to [principal fractional ideals](../../../../../../principal-fractional-ideal.md). Thus further quotienting gives the [ideal class group](../../../../../../ideal-class-group.md). The product of normalized local moduli defines $|a|_J$; at complex places the normalized modulus is the square of the ordinary absolute value. The [product formula](../../../../../../product-formula.md) says that [principal ideles](../../../../../../principal-idele.md) have modulus one. These constructions package [ideals](../../../../../../ideal.md), units and archimedean conditions into one group.

Here is the precise reciprocity equivalence. For a finite [abelian extension](../../../../../../abelian-extension.md) $L/K$, the global law is a continuous [Artin reciprocity map](../../../../../../artin-reciprocity-law.md)

$$
\theta_{L/K}:J_K\longrightarrow\operatorname{Gal}(L/K)
$$

which kills $K^*$ and sends a [uniformizer](../../../../../../uniformizer.md) [idele](../../../../../../idele.md) at an unramified place to [arithmetic Frobenius](../../../../../../frobenius-automorphism.md). Its full class-field-theoretic norm statement is $C_K/N_{L/K}C_L\cong\operatorname{Gal}(L/K)$. In the local formulation, the maps

$$
r_v:K_v^*\longrightarrow D_v\subseteq\operatorname{Gal}(L/K)
$$

are continuous, kill local units when unramified, send a local [uniformizer](../../../../../../uniformizer.md) to the same Frobenius, are compatible with restriction in towers, and obey

$$
\boxed{\prod_v r_v(a)=1\quad\text{for every }a\in K^*.}
$$

Here $D_v$ is the [decomposition group](../../../../../../decomposition-group.md) of any prime above $v$, independent of that choice because the extension is abelian. The usual local norm theorem identifies $K_v^*/N_{L_w/K_v}L_w^*$ with $D_v$. The principal-idele condition is the essential global compatibility; existence of unrelated local norm isomorphisms alone would not establish global reciprocity.

Given the compatible local maps, define

$$
\boxed{\theta((a_v))=\prod_vr_v(a_v).}
$$

Only finitely many factors are nontrivial: there are finitely many ramified places, and an [idele](../../../../../../idele.md) is a unit almost everywhere. The product is a homomorphism. Continuity follows by choosing local kernel neighbourhoods at those exceptional places and the full unit groups elsewhere. The boxed compatibility kills $K^*$, so the map descends to $C_K$. At every unramified place it has the required Frobenius value. The local norm maps also show that [idele](../../../../../../idele.md) norms are killed, since the local component of an [idele](../../../../../../idele.md) norm is $\prod_{w\mid v}N_{L_w/K_v}(b_w)$. Together with the class-field norm-index statement this gives the global norm-kernel formulation.

Conversely, embed $K_v^*$ in $J_K$ with every other component one, and set $r_v=\theta\circ\iota_v$. Each restriction is continuous and has the required unramified normalization. An open kernel of the finite-valued global map contains a basic neighbourhood whose unrestricted finite-place factors are full unit groups outside a finite set. Hence those local restrictions kill units. For an arbitrary [idele](../../../../../../idele.md), remove the finitely many exceptional and nonunit components; the remainder lies in that kernel neighbourhood. It follows directly that $\theta$ is exactly the product of its local restrictions, not merely a map agreeing on single-component [ideles](../../../../../../idele.md). Its triviality on $K^*$ is exactly the boxed product relation. With the decomposition and norm assertions of the reciprocity theorem, these restrictions are the [local reciprocity maps](../../../../../../local-artin-map.md) into $D_v$ with kernel $N_{L_w/K_v}L_w^*$.

One can explicitly connect this idelic formulation with the classical [ideal](../../../../../../ideal.md) law without assuming an idelic law in advance. A [modulus of a number field](../../../../../../modulus-of-a-number-field.md) records finitely many nonnegative exponents at finite places and a selected subset of real places. For a modulus $\mathfrak m$, let $U_{\mathfrak m}$ have factors $1+\mathfrak p_v^{m_v}$ at finite places dividing the modulus, full units at other finite places, positive real numbers at specified real places, and full infinite multiplicative groups otherwise. [Weak approximation for number fields](../../../../../../weak-approximation-for-number-fields.md) supplies a global $a\in K^*$ making $a^{-1}j$ lie in the specified local factors at the finitely many modulus places. Its [valuations](../../../../../../valuation.md) outside the modulus define an [ideal](../../../../../../ideal.md) prime to $\mathfrak m$. A different such $a$ changes that [ideal](../../../../../../ideal.md) by a ray-principal [ideal](../../../../../../ideal.md), and every [ideal](../../../../../../ideal.md) prime to $\mathfrak m$ is obtained. Hence

$$
J_K/(K^*U_{\mathfrak m})\cong I_K(\mathfrak m)/P_K(\mathfrak m).
$$

An [ideal](../../../../../../ideal.md) [Artin map](../../../../../../artin-reciprocity-law.md) killing $P_K(\mathfrak m)$ therefore extends to $J_K$ via this isomorphism; restricting it gives the local maps just constructed. Conversely, continuous local maps satisfying the product condition have an open product kernel containing some $U_{\mathfrak m}$ and hence make the [ideal](../../../../../../ideal.md) [Artin map](../../../../../../artin-reciprocity-law.md) kill $P_K(\mathfrak m)$. This proves the [idelic local-global reciprocity equivalence](../../../../../../idelic-local-global-reciprocity-equivalence.md) at the reciprocity-law level as well as the formal conversion of maps. The [arithmetic Frobenius](../../../../../../frobenius-automorphism.md) normalization and product relation agree with [Milne's local-global reciprocity formulation](https://www.jmilne.org/math/CourseNotes/CFT.pdf#page=186).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
