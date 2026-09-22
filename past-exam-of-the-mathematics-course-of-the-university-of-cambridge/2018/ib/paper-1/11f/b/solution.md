<h1 id="11f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For distinct $x,y\in U$, convexity keeps the segment $x+t(y-x)$ in $U$. Continuity of $Df$ makes

$$
q=\max_{0\leq t\leq1}\|Df(x+t(y-x))-I\|<1.
$$

The [fundamental theorem of calculus along a line segment](../../../../../../fundamental-theorem-of-calculus-along-a-line-segment.md) gives

$$
\|f(y)-f(x)-(y-x)\|\leq q\|y-x\|,
$$

so $\|f(y)-f(x)\|\geq(1-q)\|y-x\|>0$. Thus **$f$ is injective**.

The bound $\|Df(a)-I\|<1$ makes $Df(a)$ invertible by the [Neumann series](../../../../../../neumann-series.md). The inverse function theorem therefore makes $f$ locally open at every point, so $f(U)$ is open.

Surjectivity need not hold: the identity map on a proper convex open set has proper image. Even for $U=\mathbb R^n$ it can fail. In one dimension, $f(x)=\arctan x$ satisfies $|f'(x)-1|=x^2/(1+x^2)<1$, but its image is $(-\pi/2,\pi/2)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11F](../../11f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
