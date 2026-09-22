<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose $M$ with $|f|\leq M$ on $U$, and fix $r=(1-\|x\|)/4>0$. We prove a local [Lipschitz continuity](../../../../../../lipschitz-continuity.md) bound, which gives more than [continuity](../../../../../../continuous-function.md). Let $u,v\in B(x,r)$, put $d=\|v-u\|$, and suppose $d>0$. The point $w=u+(2r/d)(v-u)$ lies in $B(x,3r)\subset U$, while $d<2r$ and

$$
v=\left(1-\frac d{2r}\right)u+\frac d{2r}w.
$$

By [convexity](../../../../../../convex-function.md), $f(v)-f(u)\leq[d/(2r)](f(w)-f(u))\leq Md/r$. Interchanging $u,v$ gives

$$
\boxed{|f(v)-f(u)|\leq\frac Mr\|v-u\|\qquad(u,v\in B(x,r)).}
$$

The case $d=0$ is immediate. Every point has such a neighborhood, so **$f$ is locally Lipschitz and therefore continuous throughout $U$**. This is the [bounded convex functions are locally Lipschitz on an open ball](../../../../../../bounded-convex-functions-are-locally-lipschitz-on-an-open-ball.md) argument; no finite-dimensional assumption is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
