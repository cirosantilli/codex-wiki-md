<h1 id="e/e1/solution">Solution</h1>

↑ **Parent:** [E1](../e1.md)

A [complete metric space](../../../../complete-metric-space.md) is a [metric space](../../../../metric-space.md) in which every [Cauchy sequence](../../../../cauchy-sequence.md) converges to a point of that space.

If $x_n\to x$, choose $N$ so that $d(x_n,x)<\varepsilon/2$ for all $n\geq N$. The [triangle inequality](../../../../triangle-inequality.md) gives $d(x_m,x_n)\leq d(x_m,x)+d(x,x_n)<\varepsilon$, proving the [Cauchy sequence](../../../../cauchy-sequence.md) property.

Now let $A$ be complete in the induced [metric](../../../../metric.md). If $x\in\overline A$, choose $a_n\in A$ with $d(a_n,x)<1/n$. The sequence converges to $x$ in $X$, so is a [Cauchy sequence](../../../../cauchy-sequence.md). Completeness of $A$ supplies a limit $a\in A$. Uniqueness of limits in a [metric space](../../../../metric-space.md) gives $a=x$, hence $\overline A\subseteq A$. Therefore **a complete [metric](../../../../metric.md) subspace is closed**.

Completeness does not imply [sequential compactness](../../../../sequentially-compact-space.md). In the complete space $\mathbb R$, the sequence $x_n=n$ has no convergent [subsequence](../../../../subsequence.md): a [subsequence](../../../../subsequence.md) has strictly increasing indices $n_k\geq k$, so $x_{n_k}\to+\infty$ and is unbounded, whereas every convergent real sequence is bounded.

## ↑ Ancestors (12)

1. [E1](../e1.md)
2. [E](../../e.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
