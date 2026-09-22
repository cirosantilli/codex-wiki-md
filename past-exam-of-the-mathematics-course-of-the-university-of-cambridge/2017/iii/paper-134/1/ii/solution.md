<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $L=\mathcal O_X(D)$ and let $s_D$ be the canonical [global section](../../../../../../global-section.md) cutting out the [effective Cartier divisor](../../../../../../effective-cartier-divisor.md) $D$. The [divisor restriction exact sequence](../../../../../../divisor-restriction-exact-sequence.md) gives

$$
0\longrightarrow L^{m-1}\xrightarrow{s_D}L^m\longrightarrow L^m|_D\longrightarrow0.
$$

The hypothesis says $L|_D$ is an [ample line bundle](../../../../../../ample-line-bundle.md). By [Serre vanishing](../../../../../../serre-vanishing.md), $H^1(D,L^m|_D)=0$ for all sufficiently large $m$, so the [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) makes

$$
H^1(X,L^{m-1})\longrightarrow H^1(X,L^m)
$$

surjective for all such $m$. These are finite-dimensional [vector spaces](../../../../../../vector-space-split.md). Their dimensions form a nonincreasing sequence of nonnegative [integers](../../../../../../integer.md), so the maps are isomorphisms from some point on. Exactness then implies that the restriction

$$
H^0(X,L^m)\longrightarrow H^0(D,L^m|_D)
$$

is surjective for all sufficiently large $m$.

Choose such an $m$ for which $L^m|_D$ is also a [globally generated line bundle](../../../../../../globally-generated-line-bundle.md). Lift a generating collection of its [global sections](../../../../../../global-section.md) to $X$. At each point of $D$, one lift has nonzero image in the one-dimensional residue-field fibre, hence generates the stalk of $L^m$ by [Nakayama lemma](../../../../../../nakayama-lemma.md). Outside $D$, $s_D^m$ is nowhere zero and generates $L^m$. Together these sections generate it everywhere. Therefore

$$
\boxed{\mathcal O_X(mD)\text{ is globally generated for }m\gg0;\quad D\text{ is semiample}.}
$$

This proof works on an arbitrary [projective scheme](../../../../../../projective-scheme.md) because the defining section of an [effective Cartier divisor](../../../../../../effective-cartier-divisor.md) is a [non-zero-divisor](../../../../../../non-zero-divisor.md). If $D$ is empty, $L\cong\mathcal O_X$ and the conclusion is immediate. [Semiampleness](../../../../../../semiample-divisor.md) is the conclusion: the pullback of a line avoiding the centre of a [blowup of a smooth algebraic surface](../../../../../../blowup-of-a-smooth-algebraic-surface.md) of $\mathbb P^2$ satisfies the hypothesis on its support but has zero intersection with the exceptional curve, and therefore is not [ample](../../../../../../ample-line-bundle.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 134](../../../paper-134-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
