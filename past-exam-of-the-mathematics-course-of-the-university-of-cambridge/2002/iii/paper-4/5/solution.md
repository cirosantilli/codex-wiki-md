<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The additive [Abelian group](../../../../../abelian-group.md) $G$ is divisible because it is a real [vector space](../../../../../vector-space-split.md). Each convex subgroup $C_n$ is divisible too: for $c\ge0$ in $C_n$ and a positive integer $m$, its unique additive quotient $c/m$ satisfies $0\le c/m\le c$, hence belongs to $C_n$. Negative elements follow by taking inverses. Thus all $C_n$ are rational [vector subspaces](../../../../../vector-subspace.md), independently of whether the given real scalar multiplication respects the order.

Choose an ordered-group isomorphism $\theta_n:C_{n+1}/C_n\to\mathbb R$. It is rational-linear, since additive homomorphisms between divisible torsion-free groups preserve division by integers. Extend a rational [basis](../../../../../basis.md) of $C_n$ to one of $C_{n+1}$; equivalently choose a rational-linear section $s_n:\mathbb R\to C_{n+1}$ of $\theta_n$ composed with the quotient map. Then

$$
C_{n+1}=C_n\oplus s_n(\mathbb R).
$$

Since $C_1=0$ and the union is $G$, each $g\in G$ has a unique expression $g=\sum_{j=1}^N s_j(r_j)$ with only finitely many nonzero coefficients. Define $\Phi(g)=(r_1,r_2,\ldots)$. This is an injective additive [group homomorphism](../../../../../group-homomorphism.md). If $r_N\ne0$ is the largest active coefficient, the image of $g$ in the ordered quotient $C_{N+1}/C_N$ has sign equal to that of $r_N$. Convexity ensures that this is also the sign of $g$.

The maximum-support convention for the [Hahn group](../../../../../hahn-group.md) $V(\mathbb Z_{>0},\mathbb R)$ uses precisely finite supports and the sign of the largest active coefficient. Hence $\Phi$ preserves and reflects the [total order](../../../../../total-order.md), and therefore preserves [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md) and [meet](../../../../../greatest-lower-bound-in-a-partially-ordered-set.md). This proves the [finite-support Hahn embedding along a countable convex chain](../../../../../finite-support-hahn-embedding-along-a-countable-convex-chain.md). In fact every finite coefficient sequence is obtained, so $\Phi$ is an ordered-group isomorphism in this convention; the requested embedding follows.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
