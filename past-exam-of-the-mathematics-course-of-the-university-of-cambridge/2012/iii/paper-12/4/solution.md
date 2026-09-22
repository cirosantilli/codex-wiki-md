<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

First realize the free isometric action. Choose generators $t_1,\ldots,t_r$ of the [finitely presented group](../../../../../finitely-presented-group.md) $T$. In every dimension $d\geq3$, the [connected sum](../../../../../connected-sum-of-oriented-manifolds.md)

$$
B_d=\mathop{\#}_{j=1}^r(S^1\times S^{d-1})
$$

has [fundamental group](../../../../../fundamental-group.md) the [free group](../../../../../free-group.md) $F_r$. Map its generators onto the $t_j$ and take the connected [regular covering](../../../../../regular-covering.md) $N\to B_d$ corresponding to the kernel. Its [deck transformation group](../../../../../deck-transformation-group.md) is $F_r/\ker\pi\cong T$. Lift any [Riemannian metric](../../../../../riemannian-metric.md) on $B_d$ to $N$. [Deck transformations](../../../../../deck-transformation.md) are then [Riemannian isometries](../../../../../riemannian-isometry.md), and a [deck transformation](../../../../../deck-transformation.md) fixing one point is the identity by uniqueness of lifts. This gives the [free isometric realization of a finitely generated group](../../../../../free-isometric-realization-of-a-finitely-generated-group.md). For the trivial group use $S^d$. If $T$ is infinite the covering manifold need not be compact, which is allowed in this first construction. Simple connectivity of $N$ is not being asserted here.

**The requested nonhomeomorphism conclusion needs an extra hypothesis.** For a counterexample even with distinct [subgroups](../../../../../subgroup.md), take $T=S_3$, $U_1=\langle(1\ 2)\rangle$ and $U_2=\langle(2\ 3)\rangle$. They are conjugate and therefore [Gassman equivalent](../../../../../gassmann-equivalence.md). For every free isometric action of $T$, the conjugating element induces a [Riemannian isometry](../../../../../riemannian-isometry.md) $U_1\backslash N\to U_2\backslash N$. These quotients cannot be nonhomeomorphic. Identical [subgroups](../../../../../subgroup.md) give an even simpler obstruction. Thus the stated equivalence condition alone cannot imply the claimed topology.

A sufficient version is: for a finite $T$ with [Gassmann equivalent](../../../../../gassmann-equivalence.md), nonisomorphic [subgroups](../../../../../subgroup.md) $U_1,U_2$, there are closed isospectral manifolds with [fundamental groups](../../../../../fundamental-group.md) $U_1,U_2$, and hence they are not homeomorphic. To prove it, realize $T$ as the [fundamental group](../../../../../fundamental-group.md) of a closed smooth manifold $B$ of dimension four. Here is the needed [closed-manifold realization of a finitely presented fundamental group](../../../../../closed-manifold-realization-of-a-finitely-presented-fundamental-group.md). Start with a four-dimensional zero-handle and one one-handle for each generator. Attach two-handles along disjoint embedded boundary circles representing the relators, with arbitrary framings. The boundary is three-dimensional, so finitely many such loops can be chosen disjoint. The resulting compact handle manifold $W$ has $\pi_1(W)=T$ by the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md).

The inclusion $\partial W\to W$ is surjective on [fundamental groups](../../../../../fundamental-group.md): relative to the boundary the dual handle decomposition uses only handles of indices two, three and four, none of which introduces a fundamental-group generator. Double $W$ along its boundary. In the amalgamated product for the double, both boundary maps are the same surjection onto $T$, so the two copies of $T$ are identified completely and $\pi_1(B)=T$. The double is closed, connected and smooth after smoothing its collar. This construction works in any dimension at least four; it does not claim that every finitely presented group is a closed three-manifold group.

Let $N$ now be the [universal cover](../../../../../universal-cover.md) of $B$ with the lifted metric. Since $T$ is finite, $N$ is compact and [simply connected](../../../../../simply-connected-space.md), with a free isometric deck action of $T$. By [Sunada theorem](../../../../../sunada-theorem.md), $M_i=U_i\backslash N$ are isospectral. Because $N$ is their universal cover, $\pi_1(M_i)\cong U_i$. Nonisomorphic [fundamental groups](../../../../../fundamental-group.md) rule out a [homeomorphism](../../../../../homeomorphism.md). For an infinite $T$ the same qualified argument applies to finite-index [subgroups](../../../../../subgroup.md) with equal coset characters: divide first by the intersection $K=\operatorname{Core}_T(U_1)\cap\operatorname{Core}_T(U_2)$ of their finite-index [subgroup cores](../../../../../core-group-theory.md), producing a compact intermediate cover and a finite isometry group to which Sunada applies.

For explicit nonhomeomorphic examples, let $p$ be an odd prime. Let $H_p=(\mathbb Z/p\mathbb Z)^3$, and let $K_p$ be the [Heisenberg group over a prime field](../../../../../heisenberg-group-over-a-prime-field.md), whose elements are triples with multiplication

$$
(a,b,c)(a',b',c')=(a+a',b+b',c+c'+ab').
$$

Both have order $p^3$, and every nonidentity element has order $p$. For $K_p$, induction gives

$$
(a,b,c)^k=(ka,kb,kc+\tbinom{k}{2}ab),
$$

so the assertion follows at $k=p$, since $p$ is odd. But $H_p$ is abelian and $K_p$ is not: $(1,0,0)$ and $(0,1,0)$ do not commute.

Embed both groups regularly in $S_{p^3}$. Every nonidentity element in either [regular representation](../../../../../regular-representation.md) has cycle type $p^{p^2}$. Hence both embedded [subgroups](../../../../../subgroup.md) meet the identity class once, the class of that cycle type $p^3-1$ times, and all other classes zero times. They are [nonisomorphic Gassmann equivalent regular subgroups](../../../../../nonisomorphic-gassmann-equivalent-regular-subgroups.md). Taking $p=3$ and using the closed four-manifold construction with $T=S_{27}$ gives an explicit pair of isospectral nonhomeomorphic quotients, completing the intended construction under a sufficient hypothesis.

Finally choose distinct odd primes $p_1,\ldots,p_n$ and take

$$
T_n=\prod_{j=1}^n S_{p_j^3},\qquad
U_\epsilon=\prod_{j=1}^n L_{j,\epsilon_j},\qquad
L_{j,0}=H_{p_j},\quad L_{j,1}=K_{p_j},\quad\epsilon\in\{0,1\}^n.
$$

[Conjugacy classes](../../../../../conjugacy-class.md) in a direct product are products of classes, so their intersection counts factor. Thus all $2^n$ [subgroups](../../../../../subgroup.md) are [Gassmann equivalent](../../../../../gassmann-equivalence.md). They are pairwise nonisomorphic: the unique Sylow $p_j$-subgroup of $U_\epsilon$ is its $j$th factor, and whether it is abelian records $\epsilon_j$. Realize $T_n$ as the [fundamental group](../../../../../fundamental-group.md) of a closed four-manifold and quotient its universal cover by these [subgroups](../../../../../subgroup.md). The [binary family of nonhomeomorphic Sunada quotients](../../../../../binary-family-of-nonhomeomorphic-sunada-quotients.md) gives

$$
\boxed{2^n\text{ mutually isospectral closed four-manifolds, pairwise nonhomeomorphic and therefore nonisometric}.}
$$

This existence statement is valid; the earlier universal nonhomeomorphism assertion from Gassmann equivalence alone is not.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
