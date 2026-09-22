<h1 id="a/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $N=|G|$ and $D(U)=e(G[U])-p\binom{|U|}{2}$. For disjoint sets $U,W$ of size at least $\epsilon^2N$, the given identity and the corresponding binomial identity give

$$
|e(U,W)-p|U||W||\le|D(U\cup W)|+|D(U)|+|D(W)|<\epsilon^5N^2/3.
$$

In the nonvacuous regularity range $0<\epsilon<1$, the original sets therefore satisfy $|d(X,Y)-p|<\epsilon^3/3$. Their allowed subsets have size at least $\epsilon^2N$, so $|d(X',Y')-p|<\epsilon/3$. The triangle inequality gives

$$
|d(X',Y')-d(X,Y)|<(\epsilon+\epsilon^3)/3<\epsilon.
$$

Thus **the pair is uniform**. For $\epsilon\ge1$, the definition is vacuous or immediate; the subsequent positive-[integer](../../../../../integer-split.md) condition $k<1/\epsilon$ has no solutions.

For the partition deduction, choose $k$ equal classes of size $q=\lfloor N/k\rfloor$, putting the remainder into $V_0$. For fixed $k<1/\epsilon$ and sufficiently large $N$, $q\ge\epsilon N$ and $|V_0|<k<\epsilon N$. Every class pair is uniform by what was just proved, which is stronger than the required condition. For example, it suffices that

$$
N>\max\{k/\epsilon,\ k/(1-\epsilon k)\}.
$$

**A [graph](../../../../../graph-split.md)-size qualification is necessary if the printed deduction is read literally for every [graph](../../../../../graph-split.md) order.** Under the standard nonempty-class definition, a one-vertex [graph](../../../../../graph-split.md) satisfies the discrepancy hypothesis for every $p$ and positive $\epsilon$, but cannot be partitioned into two nonempty classes even when $2<1/\epsilon$. The source omits this small-order qualification. If $k$ divides $N$, no rounding is needed and $N\ge k$ already suffices, since $N/k>\epsilon N$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
