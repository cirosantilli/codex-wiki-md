<h1 id="e/e1/solution">Solution</h1>

↑ **Parent:** [E1](../e1.md)

A [metric space](../../../../metric-space.md) is a set $X$ with a function $d:X\times X\to[0,\infty)$ satisfying $d(x,y)=0\iff x=y$, symmetry and the [triangle inequality](../../../../triangle-inequality.md). A subset $U$ is open if every $x\in U$ has some open [open ball](../../../../open-ball.md) $B(x,r)$ contained in $U$.

For finitely many [open sets](../../../../open-set.md) $U_1,\ldots,U_k$ and $x$ in their intersection, choose radii $r_j>0$ with $B(x,r_j)\subseteq U_j$. The positive minimum radius gives a ball contained in the intersection. Thus every [finite intersection](../../../../finite-intersection.md) is open; the empty intersection is $X$, also open.

For distinct points put $\delta=d(x_1,x_2)>0$. The balls $B(x_1,\delta/3)$ and $B(x_2,\delta/3)$ are disjoint: a common point would make $d(x_1,x_2)<2\delta/3$ by the [triangle inequality](../../../../triangle-inequality.md). This proves the [Hausdorff condition](../../../../hausdorff-space.md).

A [singleton](../../../../singleton-mathematics.md) $\{x\}$ is closed because each $y\ne x$ has a ball of radius $d(x,y)/2$ avoiding it, making its complement open. [Finite unions](../../../../finite-union.md) of [closed sets](../../../../closed-set.md) are closed, as their complements are [finite intersections](../../../../finite-intersection.md) of [open sets](../../../../open-set.md). Hence **every finite subset is closed**, including the empty subset.

## ↑ Ancestors (12)

1. [E1](../e1.md)
2. [E](../../e.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
