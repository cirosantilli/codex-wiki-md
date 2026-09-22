<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [nilpotent group](../../../../../../nilpotent-group.md) has a finite [central series](../../../../../../central-series.md)

$$
1=Z_0\le Z_1\le\cdots\le Z_c=G,\qquad [G,Z_{j+1}]\le Z_j.
$$

Equivalently the [upper central series](../../../../../../upper-central-series.md), defined by $Z_{j+1}/Z_j=Z(G/Z_j)$, reaches $G$.

We first prove the [normalizer condition for nilpotent groups](../../../../../../normalizer-condition-for-nilpotent-groups.md). If $H<G$, choose the least $j$ with $Z_j\not\subseteq H$. Then $Z_{j-1}\le H$, and an element $z\in Z_j\setminus H$ satisfies $[z,H]\le Z_{j-1}\le H$. Thus $z$ normalizes $H$, giving $H<N_G(H)$.

Let $P$ be a [Sylow subgroup](../../../../../../sylow-subgroup.md) of a finite nilpotent $G$, and write $N=N_G(P)$. If $N<G$, the [normalizer](../../../../../../normalizer.md) condition gives some $g\in N_G(N)\setminus N$. The [subgroups](../../../../../../subgroup.md) $P$ and $P^g$ are both [Sylow subgroups](../../../../../../sylow-subgroup.md) of $N$, so [Sylow theorem](../../../../../../sylow-theorems.md) supplies $n\in N$ with $P^{gn}=P$. But then $gn\in N_G(P)=N$, forcing $g\in N$, a contradiction. Therefore every [Sylow subgroup](../../../../../../sylow-subgroup.md) is a [normal subgroup](../../../../../../normal-subgroup.md) of $G$.

For normal [Sylow subgroups](../../../../../../sylow-subgroup.md) $P,Q$ at different primes, $[P,Q]\le P\cap Q=1$. They commute, have coprime orders, and their product has order $|G|$. Multiplication consequently gives an isomorphism from their external [direct product of groups](../../../../../../direct-product-of-groups.md) onto $G$.

Conversely, a nontrivial [finite p-group](../../../../../../finite-p-group.md) has nontrivial [center of a group](../../../../../../center-of-a-group.md): its [class equation](../../../../../../class-equation.md) has every noncentral conjugacy-class size divisible by $p$, so $|Z(G)|$ is a positive multiple of $p$. Induction on order, applied to $G/Z(G)$, gives a central series for $G$. Finite direct products of these central series give a central series for the product, padding shorter series by the full factor. Thus the [finite nilpotent group decomposition](../../../../../../finite-nilpotent-group-decomposition.md) is

$$
\boxed{G\text{ nilpotent}\ \Longleftrightarrow\
G\cong\prod_{p\mid |G|}P_p.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
