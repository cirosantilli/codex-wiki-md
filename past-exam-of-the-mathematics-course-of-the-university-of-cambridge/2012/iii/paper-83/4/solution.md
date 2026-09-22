<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The maximum is $2^{\aleph_1}$. We construct that many [aleph-one-like linear orders](../../../../../aleph-one-like-linear-order.md), whose proper initial segments are [countable](../../../../../countable-set.md), and prove that they are nonisomorphic. As usual the rational-type requirement concerns nonempty proper initial segments; the empty segment occurs in every order.

Let $D$ be the [club set](../../../../../club-set.md) of nonzero [limit ordinals](../../../../../limit-ordinal.md) below $\omega_1$. For $S\subseteq D$, form the [order sum](../../../../../order-sum.md)

$$
L_S=\sum_{\alpha<\omega_1}B_\alpha,\qquad
B_\alpha=
\begin{cases}
1+\mathbb Q,&\alpha\in S,\\
\mathbb Q,&\alpha\notin S.
\end{cases}
$$

Here $1+\mathbb Q$ means a new least point followed by a copy of the [rational numbers](../../../../../rational-number.md); distinct blocks are disjoint, and all points of an earlier block precede every point of a later one. Every block is [countable](../../../../../countable-set.md), dense and has no greatest point. Since $0\notin S$, the full [total order](../../../../../total-order.md) has neither a least nor a greatest point. It has size $\aleph_1$.

The sum is dense: within a block use density, and for points in different blocks choose a larger point in the earlier block. If $I$ is a proper initial segment and $y\notin I$ lies in block $\alpha$, then $I$ is contained in the union of the blocks through $\alpha$. There are only countably many such blocks, each [countable](../../../../../countable-set.md). Thus $I$ is [countable](../../../../../countable-set.md), rather than an [uncountable](../../../../../uncountable-set.md) interval in an aleph-one-dense order.

Every nonempty $I$ is dense and has no least point. If it has no greatest point either, the [back-and-forth method](../../../../../back-and-forth-method.md) gives $I\cong\mathbb Q$: enumerate both orders, alternately include the least unused element from either enumeration in a finite partial [order isomorphism](../../../../../order-isomorphism.md), and choose its partner in the appropriate open interval. Density and absence of endpoints always supply a new partner. The union is a bijective order isomorphism. If $I$ has a greatest point, remove it, apply the same argument, and reattach it. Hence every nonempty proper initial segment is isomorphic to $\mathbb Q$ or $\mathbb Q+1$.

**The stationary information is recorded at the limit cuts.** Write

$$
F^S_\alpha=\bigcup_{\beta<\alpha}B_\beta.
$$

This is a continuous increasing [kappa-filtration](../../../../../kappa-filtration.md) by [countable](../../../../../countable-set.md) initial segments. At a limit $\delta$, the complement $L_S\setminus F^S_\delta$ has a least point exactly when $\delta\in S$.

Suppose $f:L_S\to L_T$ is an [order isomorphism](../../../../../order-isomorphism.md). Since each filtration stage is [countable](../../../../../countable-set.md), its image under $f$ and the corresponding image under $f^{-1}$ are bounded in block index: the supremum of their [countable](../../../../../countable-set.md) collection of [countable ordinals](../../../../../countable-ordinal.md) remains below $\omega_1$. Choose $g(\alpha)<\omega_1$ so that

$$
f[F^S_\alpha]\subseteq F^T_{g(\alpha)},\qquad
f^{-1}[F^T_\alpha]\subseteq F^S_{g(\alpha)}.
$$

The set

$$
C=\{\delta\in D:(\forall\alpha<\delta)\ g(\alpha)<\delta\}
$$

is a [club set](../../../../../club-set.md). To see unboundedness, start above any given ordinal and recursively choose $\gamma_{n+1}>\gamma_n$ larger than every $g(\alpha)$ for $\alpha\le\gamma_n$. The supremum of the [countable](../../../../../countable-set.md) sequence remains below $\omega_1$ and belongs to $C$. Closure follows because below a limit of members of $C$, each fixed $\alpha$ lies below one of those members.

For $\delta\in C$, continuity of the filtrations gives both inclusions needed for

$$
f[F^S_\delta]=F^T_\delta.
$$

The isomorphism therefore preserves whether the complementary final segment has a least point. Consequently

$$
\delta\in S\quad\Longleftrightarrow\quad\delta\in T
\qquad(\delta\in C).
$$

This [club agreement of countable filtrations](../../../../../club-agreement-of-countable-filtrations.md) proves the invariant: if $S\mathbin{\triangle}T$ is stationary, the orders cannot be isomorphic.

We also construct enough pairwise different stationary encodings. For each $\beta<\omega_1$, fix an [injection](../../../../../injective-function.md) $e_\beta:\beta\to\omega$, and set

$$
A_{\xi,n}=\{\beta\in D:\xi<\beta,\ e_\beta(\xi)=n\}.
$$

For fixed $\xi$, these sets partition the stationary tail $D\setminus(\xi+1)$. At least one $A_{\xi,n}$ is stationary: otherwise choose a club avoiding each one and intersect the countably many clubs to obtain a club avoiding the entire tail. The countable-intersection fact follows directly: above any starting point choose an increasing sequence, visiting each club infinitely often; its [countable](../../../../../countable-set.md) supremum belongs to every club by closure. For each $\xi$ let $n(\xi)$ be the least such $n$. One value $n_*$ occurs for uncountably many $\xi$, since a [countable](../../../../../countable-set.md) union of [countable](../../../../../countable-set.md) sets is [countable](../../../../../countable-set.md). For that fixed $n_*$ the cells are pairwise disjoint, by injectivity of $e_\beta$. Enumerating those cells gives

$$
(S_\eta:\eta<\omega_1),
$$

a family of pairwise disjoint stationary subsets of $D$. This is the explicit [Ulam matrix on omega-one](../../../../../ulam-matrix-on-omega-one.md) proof of [disjoint stationary subsets of omega-one](../../../../../disjoint-stationary-subsets-of-omega-one.md).

For $A\subseteq\omega_1$ put $S(A)=\bigcup_{\eta\in A}S_\eta$. If $A\ne A'$, their symmetric difference contains an entire $S_\eta$ and is stationary. The [stationary encoding in an aleph-one-like dense order](../../../../../stationary-encoding-in-an-aleph-one-like-dense-order.md) therefore produces $2^{\aleph_1}$ pairwise nonisomorphic orders $L_{S(A)}$.

Finally, on a fixed carrier of size $\aleph_1$, every total order is a subset of its Cartesian square. That square has size $\aleph_1$, so there are at most $2^{\aleph_1}$ possible relations. Thus

$$
\boxed{2^{\aleph_1}\text{ pairwise nonisomorphic orders, the maximum possible}.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
