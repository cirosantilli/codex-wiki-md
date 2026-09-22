<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If a [permutation](../../../../../../permutation.md) has disjoint cycle lengths $d_1,\ldots,d_t$, then its $k$th power is the identity exactly when every $d_j$ divides $k$. Thus its [order of a permutation](../../../../../../order-of-a-permutation.md) is $\operatorname{lcm}(d_1,\ldots,d_t)$.

Suppose $n=p^r$ is a [prime power](../../../../../../prime-power.md) and $\sigma\in S_n$ has order $n$. Each $d_j$ divides $p^r$, so is a power of $p$. Their [least common multiple](../../../../../../least-common-multiple.md) is therefore their maximum, forcing some $d_j=p^r=n$. This cycle already uses all $n$ symbols, so $\sigma$ is an $n$-cycle.

Conversely, if $n>1$ is not a [prime power](../../../../../../prime-power.md), choose a prime-power factor $a=p^r$ containing the full power of one [prime divisor](../../../../../../prime-factor.md) of $n$, and put $b=n/a$. Then $a,b>1$, they are [coprime](../../../../../../coprime-integers.md), and $ab=n$. Moreover

$$
ab-a-b=(a-1)(b-1)-1\geq0,
$$

so $a+b\leq n$. We can therefore take disjoint cycles of lengths $a$ and $b$ in $S_n$, fixing all remaining symbols. Their product has [order of a permutation](../../../../../../order-of-a-permutation.md) $\operatorname{lcm}(a,b)=ab=n$, but it is not an $n$-cycle. This proves the [prime-power characterization by full permutation cycles](../../../../../../prime-power-characterization-by-full-permutation-cycles.md):

$$
\boxed{\text{every element of order }n\text{ in }S_n\text{ is an }n\text{-cycle}\iff n=p^r.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Mathematics I](../../../mathematics-i-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
