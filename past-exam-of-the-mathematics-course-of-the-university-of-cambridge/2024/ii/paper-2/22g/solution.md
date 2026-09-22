<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

The [Baire category theorem](../../../../../baire-category-theorem.md) states that a complete metric space is not a countable union of closed sets with empty interior. To prove it, let $G_1,G_2,\ldots$ be open dense sets and start with any nonempty [open set](../../../../../open-set.md) $V$. Inductively choose closed balls

$$
\overline B(x_n,r_n)\subset
B(x_{n-1},r_{n-1})\cap G_n,
\qquad 0<r_n<2^{-n},
$$

with the first ball inside $V\cap G_1$. The centres are Cauchy. Completeness supplies a [limit](../../../../../limit-of-a-function.md) lying in every ball, hence in $V\cap\bigcap_nG_n$. Thus the intersection is dense, which is the equivalent form of the theorem.

Now each $nS$ is closed and $\bigcup_{n\geq1}nS=X$. Baire gives

$$
B(x,r)\subset nS
$$

for some $x,r,n$. Symmetry gives $B(-x,r)\subset nS$. If $\|z\|<r$, then $x+z$ and $-x+z$ lie in these two balls; convexity makes their midpoint $z$ belong to $nS$. Hence

$$
B(0,r/n)\subset S,
$$

which proves the [closed convex absorbing set has an origin neighbourhood](../../../../../closed-convex-absorbing-set-has-an-origin-neighbourhood.md) result.

Convexity cannot be dropped. In $X=\mathbb R$, set

$$
S=\{0\}\cup\bigcup_{k\geq0}
\{x:4^{-k}\leq|x|\leq2\cdot4^{-k}\}.
$$

This is closed and symmetric but has gaps arbitrarily close to zero. For any $x\ne0$, choose $k$ so that the interval

$$
\left[\frac{|x|}{2\cdot4^{-k}},\frac{|x|}{4^{-k}}\right]
$$

has length at least one, and choose an integer $n$ in it. Then $x/n\in S$, so $\bigcup_n nS=\mathbb R$, while $S$ is not a neighbourhood of zero. This is a [closed symmetric absorbing set without an origin neighbourhood](../../../../../closed-symmetric-absorbing-set-without-an-origin-neighbourhood.md).

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
