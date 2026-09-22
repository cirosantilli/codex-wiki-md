<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $p=1+\varepsilon$ and assume $\lambda>0$. The [large-deviation speed](../../../../../../large-deviation-speed.md) is $a_N=N^p$, and the answer is

$$
\boxed{I_A(x)=\begin{cases}\lambda x,&x\geq0,\\+\infty,&x<0.\end{cases}}
$$

Here and below a [large deviation principle](../../../../../../large-deviation-principle.md) at speed $a_N$ means the open-set lower bound $\liminf a_N^{-1}\log\mathbb P(X_N\in G)\geq-\inf_G I$ and the closed-set upper bound $\limsup a_N^{-1}\log\mathbb P(X_N\in F)\leq-\inf_F I$. The displayed [rate function](../../../../../../rate-function.md) is nontrivial and is a [good rate function](../../../../../../good-rate-function.md).

For $0<u<v$, the [exponential distribution](../../../../../../exponential-distribution.md) gives

$$
\mathbb P(A/a_N\in(u,v))=e^{-\lambda a_Nu}-e^{-\lambda a_Nv},
\qquad
\lim_N a_N^{-1}\log\mathbb P(A/a_N\in(u,v))=-\lambda u.
$$

Shrinking an interval about any $x>0$ supplies the local lower bound $-\lambda x$; neighborhoods of zero have [probability](../../../../../../probability.md) tending to one. Every [open set](../../../../../../open-set.md) intersecting the nonnegative half-line contains one of these neighborhoods, giving the open-set bound. If a [closed set](../../../../../../closed-set.md) $F$ contains zero, its upper bound is just $\mathbb P(\cdot)\leq1$. If it meets $[0,\infty)$ but excludes zero, closedness gives $b=\inf(F\cap[0,\infty))>0$, and $\mathbb P(A/a_N\in F)\leq e^{-\lambda a_Nb}$. A [closed set](../../../../../../closed-set.md) disjoint from the support has [probability](../../../../../../probability.md) zero. This proves the full [large deviation principle](../../../../../../large-deviation-principle.md), including the boundary at zero.

The fixed exponential tail explains the speed: an excursion of size $xN^{1+\varepsilon}$ costs $e^{-\lambda xN^{1+\varepsilon}}$. The full [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md) is unnecessary here; the limiting [cumulant-generating function](../../../../../../cumulant-generating-function.md) is flat on $\theta<\lambda$ and infinite at $\theta\geq\lambda$, so it fails the theorem's [essential smoothness](../../../../../../essential-smoothness-of-a-convex-function.md) hypothesis.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
