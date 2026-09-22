<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

The [normalizer](../../../../../normalizer.md) is $N_G(H)=\{g\in G:gHg^{-1}=H\}$. It is a [subgroup](../../../../../subgroup.md): the identity normalizes $H$, products of normalizing elements normalize it, and conjugating the equality by $g^{-1}$ proves inverse closure. The map

$$
G/N_G(H)\longrightarrow\{\text{conjugates of }H\},\qquad gN_G(H)\longmapsto gHg^{-1}
$$

is well-defined and onto. Two images are equal exactly when $g_2^{-1}g_1\in N_G(H)$, exactly the condition that their [cosets](../../../../../coset.md) coincide. Thus **the number of conjugates is $\boxed{[G:N_G(H)]}$**.

By the permitted conjugacy assertion for [Sylow subgroups](../../../../../sylow-subgroup.md), the number $n_p$ of Sylow $p$-[subgroups](../../../../../subgroup.md) equals $[G:N_G(P)]$ for one such [subgroup](../../../../../subgroup.md) $P$. [Lagrange's theorem](../../../../../lagrange-s-theorem.md) makes this divide $|G|$, and $P\subseteq N_G(P)$ also makes it divide $|G|/|P|$.

For order $72=8\cdot9$, a Sylow $3$-[subgroup](../../../../../subgroup.md) has order nine, so $n_3$ divides eight. To obtain the required congruence without assuming an additional Sylow counting theorem, let $P$ act by conjugation on the set of Sylow $3$-[subgroups](../../../../../subgroup.md). Its orbit sizes are powers of three. A fixed [subgroup](../../../../../subgroup.md) $Q$ is normalized by $P$, so $PQ$ is a [subgroup](../../../../../subgroup.md) and its order $|P||Q|/|P\cap Q|$ is a power of three. Since nine is the largest power of three dividing $72$, this forces $PQ=P=Q$. There is exactly one fixed point, namely $P$ itself. All other orbits have sizes divisible by three, giving $n_3\equiv1\pmod3$. Among $1,2,4,8$, only one and four satisfy this. Therefore **$\boxed{n_3\in\{1,4\}}$**.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
