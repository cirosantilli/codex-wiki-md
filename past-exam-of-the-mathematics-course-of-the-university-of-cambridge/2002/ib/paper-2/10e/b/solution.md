<h1 id="10e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The strict distance inequality implies $d(fx,fy)\leq d(x,y)$ for all points, so $f$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md). Hence

$$
g(x)=d(fx,x)
$$

is a [continuous function](../../../../../../continuous-function.md), since $|g(x)-g(y)|\leq d(fx,fy)+d(x,y)\leq2d(x,y)$. On the nonempty [compact metric space](../../../../../../compact-metric-space.md), $g$ attains its minimum at some $p$.

If $fp\ne p$, the strict distance inequality applied to $fp,p$ gives

$$
g(fp)=d(f^2p,fp)<d(fp,p)=g(p),
$$

a contradiction. Thus $fp=p$. If $p,q$ were different [fixed points](../../../../../../fixed-point.md), then $d(p,q)=d(fp,fq)<d(p,q)$, again impossible. **There is exactly one fixed point.** This proves [strict distance decrease on a compact metric space](../../../../../../strict-distance-decrease-on-a-compact-metric-space.md) without assuming a uniform contraction constant.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10E](../../10e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
