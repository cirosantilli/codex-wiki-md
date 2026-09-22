<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [soluble group](../../../../../solvable-group.md) is one whose [derived series](../../../../../derived-series.md) terminates: $G^{(0)}=G$, $G^{(i+1)}=[G^{(i)},G^{(i)}]$, and $G^{(r)}=1$ for some finite $r$. Each factor of this series is abelian. Conversely, if a subnormal series has abelian factors, repeated commutation moves down the series, so the [derived series](../../../../../derived-series.md) terminates. This explains the usual alternative definition in terms of abelian factors. The least $r$ is the derived length.

[Subgroups](../../../../../subgroup.md) are soluble because $H^{(i)}\leq G^{(i)}$; quotients are soluble because a [group homomorphism](../../../../../group-homomorphism.md) maps a derived [subgroup](../../../../../subgroup.md) onto the derived [subgroup](../../../../../subgroup.md) of its image. Solubility is also closed under extensions: if $N\triangleleft G$ has derived length at most $a$ and $G/N$ has length at most $b$, then $G^{(b)}\leq N$ and $G^{(a+b)}=1$. Abelian and [nilpotent groups](../../../../../nilpotent-group.md) are soluble; $S_3$ has derived [subgroup](../../../../../subgroup.md) $A_3$ and derived length two. In a [finite group](../../../../../finite-group.md), solubility is equivalent to every composition factor being cyclic of prime order: simple [soluble groups](../../../../../solvable-group.md) are abelian and therefore cyclic of prime order, while a composition series with these factors builds a [soluble group](../../../../../solvable-group.md) by extensions. This need not give an ambient-normal series with cyclic prime-order factors, which is the stronger property of supersolubility.

A [Hall subgroup](../../../../../hall-subgroup.md) for a prime set $\pi$ is a [subgroup](../../../../../subgroup.md) $H$ whose order uses only primes in $\pi$ and whose index uses only primes outside $\pi$. Its order is the full $\pi$-part of $|G|$. Sylow's theorem is the singleton-prime case; solubility allows all prime sets, although [Hall subgroups](../../../../../hall-subgroup.md) need not be normal, as the order-two [subgroups](../../../../../subgroup.md) of $S_3$ show.

Prove [Hall subgroup existence in soluble groups](../../../../../hall-subgroup-existence-in-soluble-groups.md) by induction on $|G|$. The trivial [group](../../../../../group-split.md) is immediate. Choose a nontrivial [minimal normal subgroup](../../../../../minimal-normal-subgroup.md) $N$. It is elementary abelian of some prime characteristic $p$: $N'$ is characteristic in $N$ and normal in $G$, so minimality and solubility force $N'=1$. A nontrivial [Sylow subgroup](../../../../../sylow-subgroup.md) of this finite [abelian group](../../../../../abelian-group.md) is characteristic, making $N$ a p-group. The [subgroup](../../../../../subgroup.md) of pth powers is characteristic and proper, so minimality makes it trivial. This proves [minimal normal subgroups of finite solvable groups are elementary abelian](../../../../../minimal-normal-subgroups-of-finite-solvable-groups-are-elementary-abelian.md).

By induction $G/N$ has a Hall $\pi$-subgroup $\overline H$. Let $K$ be its inverse image. Then $[G:K]$ is a $\pi'$-number. If $p\in\pi$, the whole $K$ is a $\pi$-group and is the desired [Hall subgroup](../../../../../hall-subgroup.md). If $p\notin\pi$, $K/N=Q=\overline H$ has order $s$ prime to $p$. We now prove the required complement existence explicitly, rather than invoking a splitting theorem as a substitute.

Write $N$ additively as an $\mathbb F_p$-vector space. Choose representatives $u(x)$ for $x\in Q$ with $u(1)=1$. Conjugation gives a well-defined action of $Q$ on $N$, because changing a representative by an element of the [abelian group](../../../../../abelian-group.md) $N$ does not change that action. Define $f(x,y)\in N$ by $u(x)u(y)=f(x,y)u(xy)$. Associativity yields

$$
f(x,y)+f(xy,z)=x\cdot f(y,z)+f(x,yz).
$$

Since $s$ is invertible in $\mathbb F_p$, set $c(x)=s^{-1}\sum_{z\in Q}f(x,z)$. Sum the identity over $z$ and use the bijection $z\mapsto yz$ to obtain

$$
f(x,y)=c(x)+x\cdot c(y)-c(xy).
$$

Changing representatives to $u'(x)=(-c(x))u(x)$ removes the multiplication error:

$$
u'(x)u'(y)=u'(xy).
$$

Thus $x\mapsto u'(x)$ is a homomorphic section. Its image $H$ has order $|Q|$, intersects $N$ trivially, and complements $N$ in $K$. This is [coprime splitting over an elementary abelian normal subgroup](../../../../../coprime-splitting-over-an-elementary-abelian-normal-subgroup.md). Finally $|H|$ is a $\pi$-number and $[G:H]=[G:K]|N|$ is a $\pi'$-number, so

$$
\boxed{\text{every finite soluble }G\text{ has a Hall }\pi\text{-subgroup for every prime set }\pi.}
$$

Only existence was needed here; the fuller Hall theorem also gives conjugacy and containment of arbitrary $\pi$-subgroups. Solubility makes the elementary-abelian minimal-normal induction possible and cannot simply be omitted.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
