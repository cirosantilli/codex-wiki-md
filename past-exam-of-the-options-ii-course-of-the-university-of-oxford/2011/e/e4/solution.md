<h1 id="e/e4/solution">Solution</h1>

↑ **Parent:** [E4](../e4.md)

A [metric space](../../../../metric-space.md) is [sequentially compact](../../../../sequentially-compact-space.md) if every sequence has a [convergent](../../../../convergent-sequence.md) [subsequence](../../../../subsequence.md) whose limit belongs to the space. A [limit point](../../../../limit-point.md) $\ell$ of $S$ is a point for which every open ball about $\ell$ contains a point of $S$ other than $\ell$.

Let $(x_n)$ lie in a [compact](../../../../compact-space.md) [metric space](../../../../metric-space.md). If one value occurs infinitely often, take a constant [subsequence](../../../../subsequence.md). Otherwise its set of values $S$ is infinite. If $S$ had no [limit point](../../../../limit-point.md), every point of the space would have a neighborhood containing at most one member of $S$. A finite subcover of these neighborhoods would force $S$ finite, a contradiction. Thus $S$ has a [limit point](../../../../limit-point.md); the stated [subsequence](../../../../subsequence.md) result supplies a [convergent](../../../../convergent-sequence.md) [subsequence](../../../../subsequence.md). This proves [sequential compactness](../../../../sequentially-compact-space.md).

Assume now that $X$ is nonempty, as is necessary for the requested minimum and [fixed point](../../../../fixed-point.md). The function $r(x)=d(f(x),x)$ is [continuous](../../../../continuous-function.md), as a [composition](../../../../function-composition.md) of $x\mapsto(f(x),x)$ with the [metric](../../../../metric.md). The [extreme value theorem](../../../../extreme-value-theorem.md) on a [compact space](../../../../compact-space.md) implies that $r$ attains its infimum, say at $p$. If $f(p)\neq p$, strict decrease of distances gives

$$
r(f(p))=d(f^2(p),f(p))<d(f(p),p)=r(p),
$$

contradicting minimality. Thus $f(p)=p$. If $p,q$ were distinct [fixed points](../../../../fixed-point.md), then $d(p,q)=d(f(p),f(q))<d(p,q)$, another contradiction. Hence **there is exactly one [fixed point](../../../../fixed-point.md)**. This is the [fixed point theorem for a strictly distance-decreasing map on a compact metric space](../../../../fixed-point-theorem-for-a-strictly-distance-decreasing-map-on-a-compact-metric-space.md).

[Compactness](../../../../compact-space.md) is essential. On $\mathbb R$, take

$$
\boxed{f(x)=\log(1+e^x).}
$$

Here $f(x)-x=\log(1+e^{-x})>0$, so there is no [fixed point](../../../../fixed-point.md). Nevertheless $0<f'(x)=e^x/(1+e^x)<1$ everywhere, and the [mean value theorem](../../../../mean-value-theorem.md) gives $|f(x)-f(y)|<|x-y|$ for distinct $x,y$. There is no uniform [Lipschitz](../../../../lipschitz-continuity.md) constant less than $1$, since $f'(x)\to1$ as $x\to\infty$.

## ↑ Ancestors (12)

1. [E4](../e4.md)
2. [E](../../e.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
