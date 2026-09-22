<h1 id="12f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

As printed, this part contains an indexing error. The displayed product ends at $m-1$, but the hypotheses contain $m+1$ alternating intervals indexed by $0,\ldots,m$. On the first $m$ intervals the printed polynomial has sign $(-1)^i$, while on the last interval it has sign $(-1)^{m-1}$ rather than the required $(-1)^m$. For example, when $m=1$ the printed product is the constant $Q=1$, which cannot reduce a negative extremum of $g$ on the final interval. The intended polynomial is

$$
Q(t)=(-1)^m\prod_{j=1}^{m}(t-w_j),
\qquad w_j=\frac{v_{j-1}+u_j}{2}.
$$

We prove the stated conclusion with this correction.

Each root $w_j$ lies in the gap between the $(j-1)$st and $j$th active intervals. Therefore $Q$ has sign $(-1)^i$ throughout $[u_i,v_i]$. In particular, wherever $|g|=M$, the numbers $Q$ and $g$ have the same sign, and $Q$ is nonzero.

Let

$$
K_+=\{t:g(t)=M\},\qquad K_-=\{t:g(t)=-M\}.
$$

These are [compact sets](../../../../../../compact-space.md). On their union, the [continuous function](../../../../../../continuous-function.md) $|Q|$ has a positive minimum. Hence, throughout some open neighbourhood $U$ of $K_+\cup K_-$, subtracting a sufficiently small positive multiple $\eta Q$ moves $g$ strictly towards zero and gives $|g-\eta Q|<M$. On the compact complement $[0,1]\setminus U$, continuity gives a uniform margin $|g|\leq M-\epsilon$ for some $\epsilon>0$. Taking also

$$
\eta\lVert Q\rVert_\infty<\epsilon
$$

shows that $|g-eta Q|<M$ there. Thus

$$
\lVert\eta Q-g\rVert_\infty<M
$$

for every sufficiently small $\eta>0$.

It remains to prove necessity in the [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md). Let $P$ be a best approximation of degree at most $n$, put $g=f-P$, and let $M=\lVert g\rVert_\infty$. If $g$ has no sequence of $n+2$ extrema with alternating signs, its sets of positive and negative extrema can be collected, from left to right, into $m+1$ alternating compact groups with $m\leq n$. Choose disjoint intervals $[u_i,v_i]$ containing those groups and separated by regions on which $|g|<M$. After replacing $g$ by $-g$ if necessary, they satisfy the displayed hypotheses. The corrected construction produces a polynomial $Q$ of degree $m\leq n$ and a small $\eta>0$ such that

$$
\lVert f-(P+\eta Q)\rVert_\infty
=\lVert g-\eta Q\rVert_\infty<M.
$$

This contradicts the assumed optimality of $P$. Therefore every best polynomial has the required $n+2$ alternating extrema.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [12F](../../12f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
