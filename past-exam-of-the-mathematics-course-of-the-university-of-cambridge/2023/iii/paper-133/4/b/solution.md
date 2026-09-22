<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The defining formulas imply the matching-distance identities

$$
d(z,p)=d(z,r),
\qquad
d(x,p)=d(x,q),
\qquad
d(y,q)=d(y,r).
$$

For example,

$$
d(z,r)=d(y,z)-d(y,r)
=\frac{d(x,z)+d(y,z)-d(x,y)}2
=d(z,p),
$$

and the other two follow cyclically. Thus $p,q,r$ are the [tripod points of a geodesic triangle](../../../../../../tripod-points-of-a-geodesic-triangle.md).

By the [thin geodesic triangle](../../../../../../thin-geodesic-triangle.md) condition, $p$ lies within $\delta$ of some point $p'$ on $[x,y]$ or $[y,z]$. If $p'\in[x,y]$, then the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
|d(x,p')-d(x,p)|\leq\delta.
$$

Since $q$ is the point of $[x,y]$ at distance $d(x,p)$ from $x$, the geodesic parametrization gives $d(p',q)\leq\delta$, and hence $d(p,q)\leq2\delta$. If instead $p'\in[y,z]$, comparison of distances from $z$ gives $d(p,r)\leq2\delta$.

Applying the same argument cyclically, each of $p,q,r$ lies within $2\delta$ of at least one of the other two. The graph on these three points whose edges join pairs at distance at most $2\delta$ therefore has no isolated vertex, so it is connected. Any two vertices are joined by at most two edges, and the [triangle inequality](../../../../../../triangle-inequality.md) yields

$$
\boxed{d(p,q),\ d(q,r),\ d(r,p)\leq4\delta.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
