<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is an indexing issue in the printed topology. Its cumulative sums omit $a_0$, whereas the post-slot [workload of a queue](../../../../../../workload-of-a-queue.md) in part (a) includes $a_0$. To see the problem, take all $a_t=\lambda$ for $t\leq-1$, with $\lambda<c$, and compare two inputs with $a_0=\lambda$ and $a_0=c+1$. Their distance according to the printed cumulative-sum expression is zero, yet

$$
Q_0(a,c)=0,\qquad Q_0(b,c)=1.
$$

Thus **the post-slot workload is not continuous in the literal printed topology**. On two-sided sequences that expression is a [seminorm](../../../../../../seminorm.md), since it also ignores future coordinates; the fixed-mean input class is not a [vector space](../../../../../../vector-space-split.md) (if signed inputs are allowed, it is an affine set).

The appropriate repair for the post-slot convention is to use one-sided past inputs including time zero and the [weighted cumulative-input topology for a slotted queue](../../../../../../weighted-cumulative-input-topology-for-a-slotted-queue.md):

$$
d_\#(a,b)=\sup_{n\geq1}\frac{|A_n(a)-A_n(b)|}{n+1}.
$$

This is a finite [metric](../../../../../../metric.md) on the fixed-mean class, since cumulative differences are $o(n)$; equality of all cumulative sums implies equality of all past coordinates. It is equivalent to augmenting the printed cumulative-difference distance by $|a_0-b_0|$: their cumulative sums differ only by this extra coordinate and a one-step shift.

Here is the full corrected [continuity](../../../../../../continuous-function.md) proof. Fix $a$ with $A_n(a)/n\to\lambda<c$, and let $\varepsilon=(c-\lambda)/4$. Choose $N\geq1$ such that $A_n(a)/n\leq\lambda+\varepsilon$ whenever $n\geq N$. If $d_\#(a,b)<\varepsilon/2$, then, for all such $n$,

$$
A_n(b)-cn\leq n(\lambda+\varepsilon-c)+(n+1)d_\#(a,b)
\leq n(\lambda+2\varepsilon-c)<0.
$$

Both [queue workloads](../../../../../../workload-of-a-queue.md) therefore maximize over the same finite collection $0\leq n<N$, containing the value zero. For any two finite lists, the difference of their maxima is at most the maximum absolute difference of corresponding entries. Thus

$$
\boxed{|Q_0(a,c)-Q_0(b,c)|\leq(N+1)d_\#(a,b)}
$$

in this neighborhood. In particular the [queue workload](../../../../../../workload-of-a-queue.md) is locally [Lipschitz continuous](../../../../../../lipschitz-continuity.md) and hence [continuous](../../../../../../continuous-function.md).

An alternative indexing repair retains the printed topology but interprets the time-zero function as the workload before slot $(-1,0)$, namely $\sup_{n\geq0}\{\sum_{j=1}^na_{-j}-cn\}$. The same finite-window argument proves its [continuity](../../../../../../continuous-function.md). One must then shift the time labels consistently in the later recursions. The remaining answers use the post-slot convention and $d_\#$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
