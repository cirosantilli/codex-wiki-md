<h1 id="4/2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $G=G_K$ and choose a [profinite Sylow subgroup](../../../../../../../profinite-sylow-subgroup.md) $P$ at the prime $p$. Its image in every finite quotient of $G$ is a Sylow $p$-subgroup. Put $F=K_s^P$. Every finite intermediate field $K\subseteq L\subseteq F$ has degree prime to $p$, because its corresponding open subgroup contains $P$. Condition (iii), together with the preceding Kummer reduction, gives $H^{n+1}(L,\mu_p)=0$ for each such field. The [cohomology continuity at closed subgroups](../../../../../../../cohomology-continuity-at-closed-subgroups.md) property says

$$
H^q(P,M)=\varinjlim_{P\subseteq U\subseteq G,\ U\text{ open}}H^q(U,M)
$$

for a discrete $G$-module $M$. Applying it to $M=\mu_p$ gives $H^{n+1}(P,\mu_p)=0$.

The action of the [pro-p group](../../../../../../../pro-p-group.md) $P$ on $\mu_p$ is trivial. Indeed it maps continuously to $\operatorname{Aut}(\mu_p)\cong\mathbb F_p^\times$, whose order $p-1$ is prime to $p$; every finite image of $P$ is a $p$-group, so that image is trivial. Choosing a primitive root identifies this module with the trivial module $\mathbb F_p$. Thus $H^{n+1}(P,\mathbb F_p)=0$.

We spell out why this controls arbitrary $p$-primary coefficients. A finite discrete $p$-primary $P$-module has a composition series with trivial $\mathbb F_p$ factors: its action factors through a finite $p$-group, whose only simple module in characteristic $p$ is the trivial one. Induction through the long exact cohomology sequence therefore gives vanishing of $H^{n+1}$ for every such finite module. Any discrete $p$-primary $P$-module is the filtered union of finite $P$-stable submodules. The orbit of an element is finite by continuity, and its orbit generates a finite abelian $p$-group. Continuous cohomology commutes with these filtered unions, so

$$
H^{n+1}(P,M)=0
$$

for every discrete $p$-primary module $M$. This is the mechanism behind [trivial coefficients detect the cohomological dimension of a pro-p group](../../../../../../../trivial-coefficients-detect-the-cohomological-dimension-of-a-pro-p-group.md).

Now let $M$ be any discrete $p$-primary $G$-module and $a\in H^{n+1}(G,M)$. Its restriction to $P$ is zero. Continuity at the closed subgroup $P$ makes its restriction zero in some open $U\supseteq P$. The index $m=[G:U]$ is prime to $p$, and the [restriction-corestriction identity in group cohomology](../../../../../../../restriction-corestriction-identity-in-group-cohomology.md) for the [corestriction map in group cohomology](../../../../../../../corestriction-map-in-group-cohomology.md) gives

$$
ma=\operatorname{Cor}_{U}^{G}\operatorname{Res}_{U}^{G}a=0.
$$

But $a$ has $p$-power order, so multiplication by $m$ is invertible on the cyclic group it generates. Hence $a=0$. This proves $H^{n+1}(G,M)=0$ for all discrete $p$-primary $M$. Dimension shifting through an acyclic coinduced module gives vanishing in every higher degree, which is exactly $\operatorname{cd}_p(K)\le n$.

Therefore **(iii) implies (i), completing the equivalence of all three conditions**. The key reason prime-to-$p$ extensions suffice is that they approximate a pro-$p$ Sylow subgroup, where the cyclotomic module becomes trivial; prime-to-$p$ transfer then detects every $p$-primary cohomology class.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [4](../../../4.md)
4. [Paper 21](../../../../paper-21-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
