<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Any nonzero [vector](../../../../vector.md) in $\mathbb F_2^3$ extends to a [basis](../../../../basis.md). Sending one such [basis](../../../../basis.md) to another gives an element of the [general linear group](../../../../general-linear-group.md), so its [group action](../../../../group-action-split.md) on the seven nonzero [vectors](../../../../vector.md) is a [transitive group action](../../../../transitive-group-action.md). Counting successive independent columns gives

$$
|G|=(8-1)(8-2)(8-4)=168.
$$

By the [orbit-stabilizer theorem](../../../../orbit-stabilizer-theorem.md), the [stabilizer](../../../../stabilizer-subgroup.md) $H$ of a chosen nonzero [vector](../../../../vector.md) $v$ has order $168/7=24$.

There are three two-dimensional [linear subspaces](../../../../vector-subspace.md) containing $v$, corresponding to the three one-dimensional [linear subspaces](../../../../vector-subspace.md) of $\mathbb F_2^3/\langle v\rangle$. The [stabilizer](../../../../stabilizer-subgroup.md) $H$ acts transitively on them: extend a [basis](../../../../basis.md) of either plane beginning with $v$ to a [basis](../../../../basis.md) of the whole [vector space](../../../../vector-space-split.md). Thus the [stabilizer](../../../../stabilizer-subgroup.md) of a flag $\langle v\rangle<P$ has order $24/3=8$.

If $Q\le G$ has order eight, each [orbit of a group action](../../../../orbit-group-theory.md) of $Q$ on the seven nonzero [vectors](../../../../vector.md) has size a power of two. Since seven is odd, at least one [orbit of a group action](../../../../orbit-group-theory.md) has size one. Thus $Q$ fixes a nonzero [vector](../../../../vector.md) $v$. Its [group action](../../../../group-action-split.md) on the three planes containing $v$ likewise has a fixed plane $P$. Therefore $Q$ is contained in, and by order equals, the [stabilizer](../../../../stabilizer-subgroup.md) of that flag. The [group action](../../../../group-action-split.md) of $G$ is transitive on these flags, so all such [subgroups](../../../../subgroup.md) are [conjugate subgroups](../../../../conjugate-subgroup.md).

Distinct flags give distinct [stabilizers](../../../../stabilizer-subgroup.md). In a [basis](../../../../basis.md) adapted to a flag, its order-eight [stabilizer](../../../../stabilizer-subgroup.md) consists of

$$
\begin{pmatrix}1&a&b\\0&1&c\\0&0&1\end{pmatrix},\qquad a,b,c\in\mathbb F_2.
$$

Its only common fixed nonzero [vector](../../../../vector.md) is $e_1$. Its only invariant plane is $\langle e_1,e_2\rangle$: an invariant plane is the [kernel of a linear map](../../../../kernel-of-a-linear-map-split.md) of a nonzero [linear functional](../../../../linear-functional.md), and over $\mathbb F_2$ that [linear functional](../../../../linear-functional.md) must be fixed; the displayed [matrices](../../../../matrix.md) have only the fixed nonzero [linear functional](../../../../linear-functional.md) $e_3^*$. Hence each [subgroup](../../../../subgroup.md) specifies its flag uniquely. There are seven choices of $v$ and three choices of $P$, giving

$$
\boxed{21\text{ subgroups of order }8.}
$$

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
