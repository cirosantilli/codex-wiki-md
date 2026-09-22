<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $p:N\to M=U\backslash N$ be a finite normal Riemannian covering, so $U$ acts freely by deck [isometries](../../../../../isometry.md). With $x,y$ any lifts of $\bar x,\bar y$, the [heat kernel on a finite isometric quotient](../../../../../heat-kernel-on-a-finite-isometric-quotient.md) satisfies

$$
\boxed{H_M(t,\bar x,\bar y)=\sum_{u\in U}H_N(t,x,uy).}
$$

There is no factor $1/|U|$ in this kernel formula. Simultaneous invariance of $H_N$ under [isometries](../../../../../isometry.md) proves independence of the lifts, by reindexing $U$. Each term solves the lifted [heat equation](../../../../../heat-equation.md). If $F_U$ is a [fundamental domain](../../../../../fundamental-domain.md) and $f$ a function on $M$, the integral of the right side against $f(\bar y)$ over $F_U$ equals

$$
\int_NH_N(t,x,y)f(p(y))\,dV(y),
$$

because the translates $uF_U$ tile $N$ up to sets of measure zero. This converges to $f(p(x))$ as $t\downarrow0$, proving the initial condition. Uniqueness of the [heat equation](../../../../../heat-equation.md) solution on the [closed manifold](../../../../../closed-manifold.md) gives the formula. For a noncompact finite cover, use the minimal [heat kernels](../../../../../heat-kernel.md), or compatible Friedrichs heat realizations. The normalized pullback $f\mapsto |U|^{-1/2}f\circ p$ is unitary onto the deck-invariant $L^2$ subspace and preserves the [Dirichlet energy](../../../../../dirichlet-energy.md), so it intertwines the [heat semigroups](../../../../../heat-semigroup.md) and yields the same kernel formula. No uniqueness of unrestricted noncompact heat-equation solutions is needed.

Set $I_t(g)=\int_N H_N(t,x,gx)\,dV(x)$ for an [isometry](../../../../../isometry.md) $g$. Diagonal integration and the covering degree give

$$
\boxed{Z_{U\backslash N}(t)=\frac1{|U|}\sum_{u\in U}I_t(u).}
$$

Unlike the kernel formula, the [trace](../../../../../matrix-trace.md) formula has an averaging factor: integration of a quotient function over $N$ is $|U|$ times integration over $U\backslash N$.

Suppose now $U\le T$, with $T$ any larger [group](../../../../../group-split.md) of [isometries](../../../../../isometry.md) of the [closed manifold](../../../../../closed-manifold.md) $N$. Change variables $x=hy$ and use simultaneous heat-kernel invariance to obtain

$$
I_t(hgh^{-1})=\int_NH_N(t,hy,hgy)\,dV(y)=I_t(g).
$$

Thus $I_t$ is a [class function](../../../../../class-function.md), and the [Sunada orbital heat-trace formula](../../../../../sunada-orbital-heat-trace-formula.md) can be grouped by [conjugacy classes](../../../../../conjugacy-class.md) $C$ of $T$:

$$
\boxed{Z_{U\backslash N}(t)=\sum_{C\subseteq T}\frac{|U\cap C|}{|U|}I_t(c_C),\qquad c_C\in C.}
$$

Only classes meeting the finite [subgroup](../../../../../subgroup.md) $U$ contribute, so this class sum is finite even if the larger [isometry](../../../../../isometry.md) [group](../../../../../group-split.md) $T$ is infinite.

For finite $T$, [Gassmann equivalence](../../../../../gassmann-equivalence.md) means $|U_1\cap C|=|U_2\cap C|$ for every [conjugacy class](../../../../../conjugacy-class.md). Summing these counts gives $|U_1|=|U_2|$, so the displayed formula gives identical [heat traces](../../../../../heat-trace.md). Their spectra, with [multiplicities](../../../../../multiplicity-mathematics.md), agree: as $t\to\infty$, the constant limit identifies the [multiplicity](../../../../../multiplicity-mathematics.md) of zero; after subtracting it, the slowest-decaying exponential identifies the least positive [eigenvalue](../../../../../eigenvalue.md) and its [multiplicity](../../../../../multiplicity-mathematics.md). Repeating determines every subsequent [eigenvalue](../../../../../eigenvalue.md). This proves the [Sunada theorem](../../../../../sunada-theorem.md) in the stated covering situation.

There is an important convention when the [universal cover](../../../../../universal-cover.md) $N$ has an infinite deck [group](../../../../../group-split.md) $T$. For [compact](../../../../../compact-space.md) quotient [manifolds](../../../../../topological-manifold.md), the [subgroups](../../../../../subgroup.md) must have finite index; the appropriate generalized Gassmann condition is equality of the characters of the finite coset [permutation representations](../../../../../permutation-representation.md), not equality of possibly infinite cardinalities of conjugacy-class intersections. Let $K$ be the intersection of the two [subgroup](../../../../../subgroup.md) cores. Each core is the kernel of the corresponding finite coset action, so $K$ is normal and of finite index in $T$, and $K\subseteq U_1\cap U_2$. The [manifold](../../../../../topological-manifold.md) $X=K\backslash N$ is then a [compact](../../../../../compact-space.md) finite normal cover of $M_0$. The [finite group](../../../../../finite-group.md) $G=T/K$ acts on $X$, and $H_i=U_i/K$ have equal coset [permutation characters](../../../../../permutation-character.md) in $G$. For a [finite group](../../../../../finite-group.md), the fixed-coset count is

$$
\chi_{G/H_i}(g)=\frac{|C_G(g)|}{|H_i|}\,|H_i\cap[g]|.
$$

Equality at the identity gives equal [subgroup](../../../../../subgroup.md) orders, and then equality for all $g$ gives almost-conjugacy. Applying the proved finite theorem to $H_i\backslash X=U_i\backslash N$ establishes [isospectrality](../../../../../isospectral-manifolds.md) also in this finite-index interpretation. It avoids taking the divergent [heat trace](../../../../../heat-trace.md) of a noncompact [universal cover](../../../../../universal-cover.md).

To realize a [finitely presented group](../../../../../finitely-presented-group.md) $T=\langle a_1,\ldots,a_r\mid R_1,\ldots,R_s\rangle$, begin with the [closed](../../../../../closed-set.md) smooth four-manifold $B=\#_{j=1}^r(S^1\times S^3)$, whose [fundamental group](../../../../../fundamental-group.md) is free on the $a_j$. Represent the relator words by disjoint smoothly embedded circles; general position permits this in dimension four, including separating self-intersections of representatives. Their oriented normal rank-three bundles are trivial, so perform framed surgeries replacing $S^1\times D^3$ by $D^2\times S^2$. Removing the circles' tubular neighborhoods leaves the [fundamental group](../../../../../fundamental-group.md) unchanged, by codimension-three general position. The [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md) shows that each replacement kills exactly the normal closure of its relator. The resulting [closed](../../../../../closed-set.md) smooth $M_0$ has $\pi_1(M_0)\cong T$. This gives a concrete [closed-manifold realization of a finitely presented fundamental group](../../../../../closed-manifold-realization-of-a-finitely-presented-fundamental-group.md). Equip it with any smooth [Riemannian metric](../../../../../riemannian-metric.md) and lift that metric to the universal and intermediate covers; all [covering maps](../../../../../covering-space.md) become [local isometries](../../../../../local-isometry.md).

To ensure nonisometry, one must choose nonconjugate [subgroups](../../../../../subgroup.md). If $U_1=U_2$, or they are conjugate, the quotients are [isometric](../../../../../isometry.md) for every lifted metric, so [Gassmann equivalence](../../../../../gassmann-equivalence.md) alone cannot imply nonisometry. For nonconjugate [subgroups](../../../../../subgroup.md), choose the base metric to have no nonidentity [local isometry](../../../../../local-isometry.md) between open sets, using the [Sunada local isometry lemma](../../../../../sunada-local-isometry-lemma.md) in dimension at least two. If $F:M_1\to M_2$ were an [isometry](../../../../../isometry.md), a local inverse of the first covering followed by $F$ and the second covering would be a [local isometry](../../../../../local-isometry.md) of $M_0$, hence the identity. Thus the [covering maps](../../../../../covering-space.md) satisfy $p_2F=p_1$ everywhere. Classification of connected covers then forces $U_1,U_2$ to be conjugate in $\pi_1(M_0)=T$, a contradiction. Therefore **nonconjugate almost-conjugate [subgroups](../../../../../subgroup.md) and a locally rigid base metric give isospectral nonisometric quotients**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
