<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

The strict distance inequality also gives $d(fx,fy)\le d(x,y)$ when $x=y$, so $f$ is [Lipschitz continuous](../../../../../lipschitz-continuity.md) with constant at most one, hence [continuous](../../../../../continuous-function.md). Put $g(x)=d(x,f(x))$. The [triangle inequality](../../../../../triangle-inequality.md) gives

$$
|g(x)-g(y)|\le d(x,y)+d(fx,fy)\le2d(x,y).
$$

Thus $g$ is also [Lipschitz continuous](../../../../../lipschitz-continuity.md) and [continuous](../../../../../continuous-function.md).

Assume the [compact metric space](../../../../../compact-metric-space.md) is nonempty, as needed for existence of a point. By the [extreme value theorem](../../../../../extreme-value-theorem.md), $g$ attains its infimum at some $p$. If $h=g(p)>0$, then $p\ne f(p)$, and strict distance decrease gives

$$
g(f(p))=d(f(p),f(f(p)))<d(p,f(p))=h,
$$

contradicting minimality. Since distances are nonnegative, $h=0$ and $f(p)=p$. If two different [fixed points](../../../../../fixed-point.md) $p,q$ existed, then $d(p,q)=d(f(p),f(q))<d(p,q)$, another contradiction. Therefore **there is exactly one fixed point**. This is [strict distance decrease on a compact metric space](../../../../../strict-distance-decrease-on-a-compact-metric-space.md); no uniform contraction factor less than one was assumed.

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
