<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Measure $Q_t$ immediately after service in slot $(t-1,t)$, and let $a_t\geq0$ denote work eligible for that slot's service. Writing $x^+=\max(x,0)$, the [Lindley recursion](../../../../../../lindley-recursion.md) is

$$
\boxed{Q_t=(Q_{t-1}+a_t-c)^+.}
$$

Start with an empty [queue](../../../../../../queue-queueing-theory.md) at time $-N$. Repeated substitution gives its time-zero [queue workload](../../../../../../workload-of-a-queue.md)

$$
Q_0^{(N)}(a,c)=\max_{0\leq n\leq N}\left\{\sum_{j=0}^{n-1}a_{-j}-cn\right\},
$$

where the empty sum is zero. The increasing limit defines the minimal causal [queue workload](../../../../../../workload-of-a-queue.md):

$$
\boxed{Q_0(a,c)=\sup_{n\geq0}\{A_n(a)-cn\},\qquad A_n(a)=\sum_{j=0}^{n-1}a_{-j},\quad A_0=0.}
$$

If the mean of the remote past is $\lambda<c$, then $A_n(a)/n\to\lambda$, so $A_n(a)-cn\to-\infty$. The [supremum](../../../../../../supremum.md) is then finite and is attained at a finite window. The same formula with indices shifted gives $Q_t(a,c)$ and satisfies the [Lindley recursion](../../../../../../lindley-recursion.md) directly: split the supremum into the zero-window term and all positive-window terms.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
