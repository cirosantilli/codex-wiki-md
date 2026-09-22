<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $L=d(x,y)$. If $m'$ is any other metric midpoint, apply the inequality from (a) to the chosen midpoint $m$ with $z=m'$. The right side is $\tfrac12(L/2)^2+\tfrac12(L/2)^2-L^2/4=0$, so $m=m'$. **Every pair has a unique midpoint.**

Choose successive midpoints to define $\gamma(k/2^n)$ on all dyadic parameters. Consecutive points at level $n$ have distance $L/2^n$. The [triangle inequality](../../../../../../triangle-inequality.md) gives $d(\gamma(s),\gamma(t))\leq(t-s)L$ for dyadic $s<t$. Conversely,

$$
L\leq d(x,\gamma(s))+d(\gamma(s),\gamma(t))+d(\gamma(t),y)
\leq sL+d(\gamma(s),\gamma(t))+(1-t)L,
$$

which gives the reverse bound. Thus equality holds. Completeness extends this map uniquely and continuously to $[0,1]$, retaining $d(\gamma(s),\gamma(t))=|s-t|L$. It is a constant-speed [geodesic](../../../../../../geodesic.md).

Every other [geodesic](../../../../../../geodesic.md) has the same midpoint, and then the same successive midpoints, so agrees on all dyadic parameters. [Continuity](../../../../../../continuous-function.md) gives agreement everywhere. Hence $\boxed{\text{there is exactly one geodesic segment between any two points}.}$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
