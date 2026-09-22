<h1 id="24h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the plane as $\{x:\nu\cdot x=c\}$ for a fixed unit vector $\nu$, and put $h(x)=\nu\cdot x-c$. Suppose $X$ misses the plane. Choose a point of $X$ and a number $A$ larger than its distance to the plane. The hypothesis $D_n\to\infty$ makes $\{x\in X:|h(x)|\le A\}$ bounded, and closedness of $X$ makes it compact. Thus $|h|$ attains its global minimum at some $p\in X$, with $|h(p)|>0$.

Locally the sign of $h$ is constant, and $h$ has a local minimum or maximum at $p$. Its surface gradient vanishes, so the tangent plane of $X$ there is parallel to the given plane and its normal is $\pm\nu$. For a surface tangent vector, the intrinsic Hessian of $h$ is the normal component of the [second fundamental form](../../../../../../second-fundamental-form-split.md), namely $\operatorname{Hess}_Xh=\pm b$ at $p$. The Hessian is semidefinite because this is a local extremum. Since $X$ is a [minimal surface](../../../../../../minimal-surface.md), $\operatorname{tr}_g b=2H=0$. A semidefinite symmetric form with zero trace must be zero, so $b(p)=0$. This makes $p$ a planar point, contradicting the assumption. Therefore $\boxed{X\cap\Pi\ne\varnothing}$.

The boundaryless hypothesis ensures that the minimizing point is an interior surface point. The condition on $D_n$ ensures that the infimum is attained; disjointness from a plane alone would not do so.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [24H](../../24h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
