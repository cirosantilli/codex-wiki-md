<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [topological group](../../../../../topological-group-split.md) is a [group](../../../../../group-split.md) with a [topology](../../../../../topology-split.md) for which multiplication $G\times G\to G$ and inversion $G\to G$ are continuous. A [profinite group](../../../../../profinite-group.md) has either of the following equivalent descriptions: **a [compact](../../../../../compact-space.md) [Hausdorff](../../../../../hausdorff-space.md) [totally disconnected](../../../../../totally-disconnected-space.md) [topological group](../../../../../topological-group-split.md)**, or **an [inverse limit](../../../../../inverse-limit.md) of finite discrete [groups](../../../../../group-split.md)**. [Totally disconnected](../../../../../totally-disconnected-space.md) means that every [connected component](../../../../../connected-component.md) is a singleton.

For clarity, an [inverse system](../../../../../inverse-system.md) over a [directed set](../../../../../directed-set.md) $I$ consists of [groups](../../../../../group-split.md) $G_i$ and maps $\phi_{ij}:G_j\to G_i$ for $i\le j$, with $\phi_{ii}=1$ and $\phi_{ik}=\phi_{ij}\phi_{jk}$. Its [inverse limit](../../../../../inverse-limit.md) is

$$
\varprojlim G_i=\{(g_i)\in\prod_iG_i:\phi_{ij}(g_j)=g_i\text{ whenever }i\le j\},
$$

with coordinatewise multiplication and the [subspace topology](../../../../../subspace-topology.md). Equivalently, it is a [group](../../../../../group-split.md) with compatible continuous projections such that every other compatible family of maps into the $G_i$ factors uniquely through it.

The displayed limit is a [closed subgroup](../../../../../closed-subgroup.md) of the [compact](../../../../../compact-space.md) [Hausdorff](../../../../../hausdorff-space.md) product of the [finite groups](../../../../../finite-group.md), and is [totally disconnected](../../../../../totally-disconnected-space.md), since two different tuples are separated by a [clopen](../../../../../clopen-set.md) coordinate condition. Conversely a [compact](../../../../../compact-space.md) [Hausdorff](../../../../../hausdorff-space.md) [totally disconnected](../../../../../totally-disconnected-space.md) [group](../../../../../group-split.md) has a [neighbourhood basis](../../../../../neighbourhood-basis.md) of [open normal subgroups](../../../../../open-normal-subgroup.md). One way to see the [group](../../../../../group-split.md) part of this standard clopen-basis fact is to choose a [clopen](../../../../../clopen-set.md) identity [neighbourhood](../../../../../neighbourhood-mathematics.md) $U$ inside a prescribed [neighbourhood](../../../../../neighbourhood-mathematics.md). [Compactness](../../../../../compact-space.md) of $U$ and [continuity](../../../../../continuous-function.md) give a symmetric identity [neighbourhood](../../../../../neighbourhood-mathematics.md) $V$ with $VU\subseteq U$. The stabilizer $H=\{g:gU=U\}$ contains $V$, is open, and is contained in $U$ because $1\in U$. Its index is finite by part (ii); its [normal core](../../../../../core-group-theory.md) is the intersection of finitely many conjugates and is open and normal. The canonical map

$$
G\longrightarrow\varprojlim_{N\trianglelefteq_oG}G/N
$$

is [injective](../../../../../injective-function.md) because these $N$ separate points, and [surjective](../../../../../surjective-function.md) because compatible [cosets](../../../../../coset.md) have the [finite intersection property](../../../../../finite-intersection-property.md) and $G$ is [compact](../../../../../compact-space.md). It is a [homeomorphism](../../../../../homeomorphism.md) by [compactness](../../../../../compact-space.md) and the [Hausdorff](../../../../../hausdorff-space.md) property. This explains the equivalence of the two definitions.

The [profinite Frattini subgroup](../../../../../profinite-frattini-subgroup.md) is $\Phi(G)=\bigcap M$, where $M$ ranges over all maximal proper [open subgroups](../../../../../open-subgroup.md); for the trivial [group](../../../../../group-split.md) the empty intersection is $G$. For a [pro-p group](../../../../../pro-p-group.md),

$$
\boxed{\Phi(G)=\overline{G^p[G,G]}.}
$$

Here powers and [group commutators](../../../../../group-commutator.md) mean generated [subgroups](../../../../../subgroup.md) and the bar supplies [closure](../../../../../closure-topology.md). Every maximal [open subgroup](../../../../../open-subgroup.md) in a [pro-p group](../../../../../pro-p-group.md) is normal of index $p$, as follows by passing to the [finite p-group](../../../../../finite-p-group.md) quotient by its [normal core](../../../../../core-group-theory.md). Such a [subgroup](../../../../../subgroup.md) therefore contains all powers and [group commutators](../../../../../group-commutator.md). Conversely the quotient by $D=\overline{G^p[G,G]}$ is an abelian [pro-p group](../../../../../pro-p-group.md) of exponent $p$. If an element of this quotient is nontrivial, some finite [elementary abelian](../../../../../elementary-abelian-group.md) quotient detects it; a [linear functional](../../../../../linear-functional.md) to $\mathbb F_p$ then detects it as well. Its [group homomorphism kernel](../../../../../kernel-of-a-group-homomorphism.md) pulls back to a maximal [open subgroup](../../../../../open-subgroup.md) of $G$. Thus the intersection of these kernels is exactly $D$.

We also use the topological generation criterion: a subset generates $G$ topologically if and only if its image generates $G/\Phi(G)$ topologically. To prove the nontrivial direction, a proper closed generated [subgroup](../../../../../subgroup.md) $K$ lies in a proper [open subgroup](../../../../../open-subgroup.md) $KN$ for a suitably small open normal $N$, and hence in a maximal [open subgroup](../../../../../open-subgroup.md) obtained from the finite quotient $G/N$. Since that maximal [subgroup](../../../../../subgroup.md) contains $\Phi(G)$, the image of $K$ cannot generate the [Frattini quotient](../../../../../frattini-quotient.md).

Now suppose $G$ is a nontrivial procyclic [pro-p group](../../../../../pro-p-group.md). If it had distinct maximal [open subgroups](../../../../../open-subgroup.md) $M_1,M_2$, the [homomorphism](../../../../../homomorphism.md) to $C_p\times C_p$ induced by the two quotient maps would be onto: its projections are onto, and a proper such [subgroup](../../../../../subgroup.md) would be a one-dimensional graph, forcing the two kernels to coincide. Hence $G/(M_1\cap M_2)\cong C_p^2$, contradicting procyclicity. Thus there is exactly one maximal [open subgroup](../../../../../open-subgroup.md) $M$, and $\Phi(G)=M$. Any $g\notin M$ generates $G/\Phi(G)\cong C_p$, so the criterion gives

$$
\boxed{G=\overline{\langle g\rangle}.}
$$

For the trivial [group](../../../../../group-split.md) use its identity as generator. **The additive [group](../../../../../group-split.md) $\mathbb Z_p$ is an infinite example**, topologically generated by $1$: its finite continuous quotients are cyclic $\mathbb Z/p^n\mathbb Z$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
