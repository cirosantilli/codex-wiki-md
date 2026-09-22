<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In level $n$, each group is

$$
2^{-(n+1)}+2^{-(n+1)}-2^{-n}=0,
$$

and there are $2^n$ such groups. The [partial sums](../../../../../../../partial-sum.md) at completed groups are therefore zero. Inside a group of level $n$, the only other [partial sums](../../../../../../../partial-sum.md) are $2^{-(n+1)}$ and $2^{-n}$. Every level contains finitely many terms, so the level containing the $N$th term tends to infinity with $N$. Thus all [partial sums](../../../../../../../partial-sum.md) lie between zero and a bound tending to zero. By the [squeeze theorem](../../../../../../../squeeze-theorem.md), the [series](../../../../../../../series-mathematics.md) has sum $\boxed{0}$.

For the next two parts, label the positive occurrences of size $2^{-(n+1)}$ by $P_n$ and the negative occurrences of size $-2^{-n}$ by $N_n$. There are exactly $2^{n+1}$ occurrences in $P_n$ and $2^n$ in $N_n$. Occurrences with equal value retain separate labels, so checking their counts verifies a [bijection](../../../../../../../bijection.md) of terms.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
