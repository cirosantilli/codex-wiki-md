<h1 id="10d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The upper bound follows immediately from [convexity](../../../../../../convex-function.md), since

$$
y_0+\lambda r=(1-\lambda)y_0+\lambda(y_0+r).
$$

For the lower bound, write

$$
y_0=\frac1{1+\lambda}(y_0+\lambda r)
+\frac\lambda{1+\lambda}(y_0-r).
$$

Applying convexity and rearranging gives

$$
\boxed{(1+\lambda)f(y_0)-\lambda f(y_0-r)
\leq f(y_0+\lambda r)
\leq(1-\lambda)f(y_0)+\lambda f(y_0+r)}.
$$

Choose a fixed $r_0>0$ with $[y_0-r_0,y_0+r_0]\subset(a,b)$. Applying these bounds with $r=r_0$ and $r=-r_0$ shows that the difference $f(y_0+h)-f(y_0)$ is trapped between quantities of order $|h|/r_0$. Both tend to zero, so every [convex function](../../../../../../convex-function.md) on an open interval is continuous.

Now suppose $c$ is a local minimum but some $x$ satisfies $f(x)<f(c)$. For sufficiently small $\lambda>0$, the point $z=(1-\lambda)c+\lambda x$ lies in the neighbourhood on which $c$ is minimal, whereas convexity gives

$$
f(z)\leq(1-\lambda)f(c)+\lambda f(x)<f(c),
$$

a contradiction. Thus

$$
\boxed{f(x)\geq f(c)\text{ for every }x\in(a,b)}.
$$

Differentiability at the minimizer is unnecessary: $f(x)=|x-c|$ is convex, has its global minimum at $c$, and is not differentiable there.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10D](../../10d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
