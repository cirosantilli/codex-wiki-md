<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [soluble group](../../../../../solvable-group.md) is a [group](../../../../../group-split.md) whose [derived series](../../../../../derived-series.md) $G^{(0)}=G$, $G^{(i+1)}=[G^{(i)},G^{(i)}]$ terminates at $1$. Equivalently, it has a finite [subnormal series](../../../../../subnormal-series.md) with abelian factors. For the reverse implication, if $G/N$ has derived length $r$, then $G^{(r)}\le N$; if $N$ has derived length $s$, then $G^{(r+s)}=1$. Iterating this observation through the series proves the equivalence. For a finite [group](../../../../../group-split.md), refining the abelian factors to [composition factors](../../../../../composition-factor.md) says that solubility is equivalent to all [composition factors](../../../../../composition-factor.md) being cyclic of prime order.

[Subgroups](../../../../../subgroup.md) and [quotient groups](../../../../../quotient-group.md) of [soluble groups](../../../../../solvable-group.md) are soluble, since their [derived series](../../../../../derived-series.md) lie in, or are images of, the original series. The same calculation proves closure under [group extensions](../../../../../group-extension.md). [Finite p-groups](../../../../../finite-p-group.md) are [nilpotent groups](../../../../../nilpotent-group.md), hence soluble: their nontrivial centers allow induction to construct a [central series](../../../../../central-series.md). Every finite [nilpotent group](../../../../../nilpotent-group.md) is a [direct product of groups](../../../../../direct-product-of-groups.md) of its [Sylow subgroups](../../../../../sylow-subgroup.md). The converse fails: $S_3$ has the abelian-factor series $1<C_3<S_3$, but its order-two [Sylow subgroups](../../../../../sylow-subgroup.md) are not normal. The [symmetric group](../../../../../symmetric-group.md) $S_4$ is also soluble, with series $1<V_4<A_4<S_4$ and abelian factors. A finite [soluble group](../../../../../solvable-group.md) has elementary abelian [minimal normal subgroups](../../../../../minimal-normal-subgroup.md), by the argument in 1(c). In contrast, a nonabelian [simple group](../../../../../simple-group.md) is a [perfect group](../../../../../perfect-group.md) and is not soluble.

The [Fitting subgroup](../../../../../fitting-subgroup.md) collects the normal nilpotent structure. For a nontrivial finite [soluble group](../../../../../solvable-group.md) it is nontrivial, since it contains an elementary abelian [minimal normal subgroup](../../../../../minimal-normal-subgroup.md). Part 1(c) proves $C_G(F)\le F$, so [conjugation](../../../../../conjugation.md) embeds $G/C_G(F)$ in $\operatorname{Aut}(F)$. This shows why controlling a [soluble group](../../../../../solvable-group.md) through normal abelian or nilpotent layers is effective, even when the whole [group](../../../../../group-split.md) is not a [nilpotent group](../../../../../nilpotent-group.md).

For a set of primes $\pi$, a [Hall subgroup](../../../../../hall-subgroup.md) of type $\pi$ has order divisible only by primes in $\pi$ and index divisible only by primes outside $\pi$. The [Hall theorem for soluble groups](../../../../../hall-conjugacy-and-embedding-in-finite-soluble-groups.md) says that a finite [soluble group](../../../../../solvable-group.md) has such [subgroups](../../../../../subgroup.md), any two are conjugate, and every [subgroup](../../../../../subgroup.md) of $\pi$-order is contained in one. These assertions generalize the [Sylow theorems](../../../../../sylow-theorems.md), which treat a single prime. Here is a proof of all three assertions.

First we need [coprime splitting over an elementary abelian normal subgroup](../../../../../coprime-splitting-over-an-elementary-abelian-normal-subgroup.md). Suppose $V\trianglelefteq E$ is an elementary abelian p-group and $Q=E/V$ has order $h$ prime to $p$. A section $s:Q\to E$ defines an action on $V$ and an additive factor set $f(x,y)$ by $s(x)s(y)=f(x,y)s(xy)$. Associativity says

$$
f(x,y)+f(xy,z)=x f(y,z)+f(x,yz).
$$

Summing over $z\in Q$ and dividing by $h$ in $V$ gives $f(x,y)=b(x)+xb(y)-b(xy)$, where $b(x)=h^{-1}\sum_zf(x,z)$. Replacing $s(x)$ by $-b(x)s(x)$ removes the factor set, giving a complement. Two complements differ by a map $d$ satisfying $d(xy)=d(x)+xd(y)$. Averaging over $y$ gives $d(x)=b-xb$, so the complements are conjugate by an element of $V$. This proves both splitting and conjugacy, without assuming that an arbitrary extension splits.

Induct on $|G|$, taking an elementary abelian [minimal normal subgroup](../../../../../minimal-normal-subgroup.md) $V$ of exponent $p$. Choose a quotient [Hall subgroup](../../../../../hall-subgroup.md) $\bar H\le G/V$ and let $K$ be its preimage. If $p\in\pi$, then $K$ itself is a [Hall subgroup](../../../../../hall-subgroup.md). If $p\notin\pi$, the preceding splitting argument gives a complement $H$ to $V$ in $K$, and that complement is a [Hall subgroup](../../../../../hall-subgroup.md) of $G$.

For conjugacy, the images of two [Hall subgroups](../../../../../hall-subgroup.md) are quotient [Hall subgroups](../../../../../hall-subgroup.md), so induction allows them to have the same [image](../../../../../image-of-a-function.md) and lie in the same $K$. If $p\in\pi$, every [Hall subgroup](../../../../../hall-subgroup.md) contains $V$: its product with $V$ is a $\pi$-subgroup and cannot be larger by the subgroup-order formula. Both are then $K$. If $p\notin\pi$, both are complements to $V$ in $K$, so the averaging argument conjugates them.

Finally let $U\le G$ be any $\pi$-subgroup. By induction its [image](../../../../../image-of-a-function.md) lies in a quotient [Hall subgroup](../../../../../hall-subgroup.md), so $U\le K$. If $p\in\pi$, $K$ is already a [Hall subgroup](../../../../../hall-subgroup.md) containing $U$. Otherwise write $K=V\rtimes H$. In $VU$, both $U$ and the inverse [image](../../../../../image-of-a-function.md) in $H$ of the [image](../../../../../image-of-a-function.md) of $U$ are complements to $V$. Complement conjugacy therefore places $U$ in a conjugate of $H$. This proves embedding and completes the induction.

**Thus existence, conjugacy and containment all hold for every prime set in a finite [soluble group](../../../../../solvable-group.md).** The solubility hypothesis matters: $A_5$ has no [Hall subgroup](../../../../../hall-subgroup.md) for $\pi=\{2,5\}$. Such a [subgroup](../../../../../subgroup.md) would have index three; its coset action would give a nontrivial [group homomorphism](../../../../../group-homomorphism.md) $A_5\to S_3$, impossible because $A_5$ is a [simple group](../../../../../simple-group.md) and has order $60$. This example also distinguishes a [Hall subgroup](../../../../../hall-subgroup.md) from a merely arbitrary [subgroup](../../../../../subgroup.md) whose order uses the chosen primes.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
