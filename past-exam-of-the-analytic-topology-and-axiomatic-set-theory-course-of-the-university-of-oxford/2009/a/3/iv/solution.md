<h1 id="a/3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $T_n=h(\{x\in\mathbb R:|x|>n\})$, making explicit that these are [subsets](../../../../../subset.md) of $Y$. If $p\notin h[\mathbb R]$ and $U$ is an open [neighbourhood](../../../../../neighbourhood-mathematics.md) of $p$, then $h([-n,n])$ is [compact](../../../../../compact-space.md) and hence closed in $Y$. The [open set](../../../../../open-set.md) $U\setminus h([-n,n])$ still contains $p$ and meets the [dense](../../../../../dense-set.md) image of $h$. Such an [intersection](../../../../../set-intersection.md) point belongs to $T_n$, so $p\in\overline{T_n}$ for every $n$.

Conversely, if $p=h(x)$ choose an integer $n>|x|$. Since $h$ is an [embedding](../../../../../topological-embedding.md), there is an open [neighbourhood](../../../../../neighbourhood-mathematics.md) $U$ of $p$ in $Y$ whose [intersection](../../../../../set-intersection.md) with $h[\mathbb R]$ is $h((-n,n))$. It misses $T_n$, so $p\notin\overline{T_n}$. Hence

$$
\boxed{Y\setminus h[\mathbb R]=\bigcap_{n\in\omega}\overline{T_n}^{\,Y}.}
$$

For the [two ends of a real-line compactification](../../../../../two-ends-of-a-real-line-compactification.md), let $A_n^+=\overline{h((n,\infty))}$ and $A_n^-=\overline{h((-\infty,-n))}$. Each is nonempty [compact](../../../../../compact-space.md) and [connected](../../../../../connected-space.md), being the [closure](../../../../../closure-topology.md) of a [connected](../../../../../connected-space.md) image. The two nested families therefore have nonempty [connected](../../../../../connected-space.md) intersections $C^+$ and $C^-$. Since [closure](../../../../../closure-topology.md) commutes with finite unions, $\overline{T_n}=A_n^+\cup A_n^-$. Moreover

$$
\bigcap_n(A_n^+\cup A_n^-)=C^+\cup C^-.
$$

For if a point fails both intersections, it fails one positive member and one negative member, hence both members at the larger index by nesting.

If the remainder were a finite three-point [set](../../../../../set-split.md), its Hausdorff [subspace topology](../../../../../subspace-topology.md) would be discrete. Each nonempty [connected subset](../../../../../connected-subset.md) $C^\pm$ would then be a [singleton](../../../../../singleton-mathematics.md), so their [union](../../../../../set-union.md) would have at most two points. This contradiction proves **there is no three-point [Hausdorff compactification](../../../../../hausdorff-compactification.md) of the [real line](../../../../../real-line.md)**. The argument does not assert that every possible remainder is finite.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
