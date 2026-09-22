<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Factor the [group order](../../../../order-of-a-finite-group.md) as $588=2^2\cdot3\cdot7^2$. The [Sylow theorems](../../../../sylow-theorems.md) say that the number of [Sylow subgroups](../../../../sylow-subgroup.md) for the prime seven divides $12$ and is congruent to one modulo seven. Among $1,2,3,4,6,12$, only one qualifies. Thus there is a unique [normal subgroup](../../../../normal-subgroup.md) $N$ of order $49$.

Every [group](../../../../group-split.md) of prime-square order is [Abelian](../../../../abelian-group.md). Indeed its [center of a group](../../../../center-of-a-group.md) is nontrivial, and a cyclic quotient by the [center of a group](../../../../center-of-a-group.md) forces the whole [group](../../../../group-split.md) to be abelian. Consequently $N$ is either $C_{49}$ or $C_7\times C_7$, and in either case it has two [composition factors](../../../../composition-factor.md), both $C_7$.

It remains to consider $Q=H/N$, of order twelve. Its number of [Sylow subgroups](../../../../sylow-subgroup.md) for the prime three is either one or four:

- If it is one, the normal order-three [subgroup](../../../../subgroup.md) has factor $C_3$, and the remaining quotient has order four. An order-four [group](../../../../group-split.md) is abelian and has two factors $C_2$.
- If it is four, these order-three [subgroups](../../../../subgroup.md) have disjoint nonidentity elements and account for eight elements. Any [Sylow subgroup](../../../../sylow-subgroup.md) for the prime two, of order four, must consist of the four remaining elements, since its nonidentity elements have power-of-two orders. It is therefore unique and normal. Its two factors are $C_2$, and the quotient has order three, giving $C_3$.

Lift the [composition series](../../../../composition-series.md) of $Q$ to $H$ using the [subgroup correspondence theorem](../../../../subgroup-correspondence-theorem.md), and join it to a [composition series](../../../../composition-series.md) inside $N$. This gives

$$
\boxed{C_2,\ C_2,\ C_3,\ C_7,\ C_7}
$$

as the multiset of [composition factors](../../../../composition-factor.md). The [Jordan–Hölder theorem](../../../../jordan-holder-theorem.md) makes this independent of the chosen series. In particular every [group](../../../../group-split.md) of order $588$ is a [solvable group](../../../../solvable-group.md), with composition length five; that is a statement about composition length, not necessarily its [derived length](../../../../derived-length.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
