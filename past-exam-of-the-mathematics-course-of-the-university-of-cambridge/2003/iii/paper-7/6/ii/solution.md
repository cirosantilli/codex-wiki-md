<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $m=|A|$, choose $u=\lfloor N^{3/4}\rfloor$, and let $A_i$ count the points of $A$ in the length-$u$ window ending at $i$, for $1\leq i\leq N+u$. Each element occurs in precisely $u$ such windows, so $\sum_i A_i=um$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) consequently gives

$$
\sum_i\binom{A_i}2=\frac12\left(\sum_iA_i^2-um\right)\geq\frac12\left(\frac{u^2m^2}{N+u}-um\right).
$$

On the other hand, a pair $a<b$ of difference $d=b-a<u$ belongs to exactly $u-d$ windows; larger differences contribute none. The [Sidon set](../../../../../../sidon-set.md) condition permits at most one pair for each positive difference $d$. Therefore

$$
\sum_i\binom{A_i}2\leq\sum_{d=1}^{u-1}(u-d)=\frac{u(u-1)}2.
$$

Combining these two estimates proves the [sliding-window upper bound for Sidon sets](../../../../../../sliding-window-upper-bound-for-sidon-sets.md):

$$
m^2\leq(N+u)\left(1-\frac1u+\frac mu\right)\leq N+u+\frac{N+u}{u}m.
$$

If $D=(N+u)/u$, the final inequality for this [quadratic polynomial](../../../../../../quadratic-polynomial.md) implies $m\leq\sqrt{N+u}+D$; otherwise $m(m-D)>N+u$. With the chosen $u$, $D=O(N^{1/4})$ and $\sqrt{N+u}=\sqrt N+O(N^{1/4})$. Thus

$$
\boxed{|A|\leq\sqrt N+O(N^{1/4})=\sqrt N+o(\sqrt N).}
$$

Together with part (i)'s construction, this proves that the maximum [cardinality](../../../../../../cardinality.md) is **$\sqrt N+o(\sqrt N)$**. The lower and upper error terms need not have the same size to establish that asymptotic conclusion.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
