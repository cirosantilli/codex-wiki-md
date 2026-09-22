<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

The [intermediate value theorem](../../../../../intermediate-value-theorem.md) says that if $f:[a,b]\to\mathbb R$ is a [continuous function](../../../../../continuous-function.md), every value between $f(a)$ and $f(b)$ is attained at some point of $[a,b]$.

For a proof, endpoint values are immediate, and replacing $f$ by $-f$ reduces the remaining case to $f(a)<y<f(b)$. The set $S=\{x\in[a,b]:f(x)\le y\}$ is nonempty and bounded above; let $c=\sup S$ by the [least-upper-bound property](../../../../../least-upper-bound-property.md). [Continuity](../../../../../continuous-function.md) and the strict endpoint inequalities ensure $a<c<b$: near $a$ there are points in $S$, and near $b$ there are none. If $f(c)>y$, [continuity](../../../../../continuous-function.md) gives a neighborhood of $c$ containing no points of $S$, contradicting the defining approximation property of the [supremum](../../../../../supremum.md). If $f(c)<y$, [continuity](../../../../../continuous-function.md) gives points to the right of $c$ still in $S$, contradicting its being an upper bound. Hence $f(c)=y$, proving the [intermediate value theorem](../../../../../intermediate-value-theorem.md).

For the distance problem, define the [continuous function](../../../../../continuous-function.md)

$$
d(x)=\sqrt{(x-a)^2+(f(x)-b)^2}.
$$

It satisfies $d(x)\ge|x-a|$, so it is a [coercive function](../../../../../coercive-function.md): $d(x)\to\infty$ as $|x|\to\infty$. Choose $R>|a|+d(0)+1$. Outside $[-R,R]$, the distance is greater than $d(0)$. On $[-R,R]$, the [extreme value theorem](../../../../../extreme-value-theorem.md) gives a minimizer $x_0$, with $A=d(x_0)\le d(0)$. It is therefore a global minimizer and $A\ge0$.

For any $y>A$, choose $X>x_0$ so large that $d(X)>y$. Apply the [intermediate value theorem](../../../../../intermediate-value-theorem.md) to $d$ on $[x_0,X]$ to obtain a point whose distance is $y$. The distance $A$ itself is attained at $x_0$, and no smaller value is possible. This is the [range of a continuous coercive real function](../../../../../range-of-a-continuous-coercive-real-function.md). Thus **the distance set is exactly**

$$
\boxed{[A,\infty),\qquad A=\min_{x\in\mathbb R}\sqrt{(x-a)^2+(f(x)-b)^2}.}
$$

In particular $A=0$ precisely when the fixed point lies on the graph.

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
