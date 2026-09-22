<h1 id="b/5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First establish the two general claims about [polycyclic groups](../../../../../../polycyclic-group.md). Intersect a subnormal cyclic-factor series $(G_i)$ with $H\leq G$. Then $H\cap G_i\trianglelefteq H\cap G_{i+1}$, and the inclusion induces an [injective](../../../../../../injective-function.md) homomorphism

$$
\frac{H\cap G_{i+1}}{H\cap G_i}\longrightarrow\frac{G_{i+1}}{G_i}.
$$

A subgroup of a [cyclic group](../../../../../../cyclic-group.md) is cyclic, so this is a cyclic-factor [subnormal series](../../../../../../subnormal-series.md) for $H$, after omitting repetitions. This proves [subgroups of polycyclic groups are polycyclic](../../../../../../subgroups-of-polycyclic-groups-are-polycyclic.md).

To prove the generator bound, choose $g_i\in G_i$ whose coset generates $G_i/G_{i-1}$ whenever that factor is nontrivial. Inductively $G_i=\langle G_{i-1},g_i\rangle$, so $G=\langle g_1,\ldots,g_n\rangle$. This is the [generator bound from a cyclic-factor series](../../../../../../generator-bound-from-a-cyclic-factor-series.md): **at most $n$ generators suffice**.

For the first example, take $G=C_2^m$ with its coordinate flag

$$
0<C_2<C_2^2<\cdots<C_2^m.
$$

It has length exactly $m$ and each factor is $C_2$, so all factors are cyclic.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the algebra course of the University of Oxford](../../../../../split.md)
7. [Algebra course of the University of Oxford](../../../../../../algebra-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
