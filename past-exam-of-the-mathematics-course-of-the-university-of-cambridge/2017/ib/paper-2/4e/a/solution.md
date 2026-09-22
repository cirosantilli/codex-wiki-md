<h1 id="4e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [continuity](../../../../../../continuous-function.md) condition at $x\in X$ between [metric spaces](../../../../../../metric-space.md) is

$$
\boxed{\forall\epsilon>0\ \exists\delta>0:\quad d(x,y)<\delta\Longrightarrow e(f(x),f(y))<\epsilon.}
$$

The function is continuous when this holds at every $x$.

If $f$ is continuous and $U\subseteq Y$ is an [open set](../../../../../../open-set.md), take $x\in f^{-1}(U)$. Some $\epsilon$-ball around $f(x)$ lies in $U$. Continuity gives a $\delta$-ball around $x$ mapped into that ball and hence contained in $f^{-1}(U)$. Thus $f^{-1}(U)$ is open, including the empty set, in the notation for the [image and preimage of a function](../../../../../../image-and-preimage-of-a-function.md).

Conversely, suppose every open set has open preimage. For fixed $x$ and $\epsilon>0$, the preimage of the open ball $B_e(f(x),\epsilon)$ is open and contains $x$, so contains some $B_d(x,\delta)$. This gives the displayed metric definition. Therefore $\boxed{f\text{ is continuous}\iff f^{-1}(U)\text{ is open for every open }U}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4E](../../4e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
