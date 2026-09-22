<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In an [irreducible topological space](../../../../irreducible-topological-space.md), any two nonempty [open subsets](../../../../open-set.md) intersect. Let $W\subseteq X$ be a nonempty [open subset](../../../../open-set.md). Two nonempty subsets open in $W$ are also open in $X$, and hence intersect; thus $W$ is itself an [irreducible topological space](../../../../irreducible-topological-space.md). If $W$ were disconnected, a separation into two disjoint nonempty [open subsets](../../../../open-set.md) would contradict this intersection property. Hence $W$ is a [connected space](../../../../connected-space.md). The empty [open subset](../../../../open-set.md) is connected as well under the usual convention.

Discard empty members of $\mathcal U$ as in (b). Every finite intersection $U_{i_0}\cap\cdots\cap U_{i_q}$ is nonempty by repeated use of the intersection property and is an [open subset](../../../../open-set.md), hence a [connected space](../../../../connected-space.md). A [locally constant function](../../../../locally-constant-function.md) on this intersection is constant. It follows that the [constant sheaf](../../../../constant-sheaf.md) has

$$
\underline A(U_{i_0}\cap\cdots\cap U_{i_q})\cong A,
$$

and every restriction map between these nonempty intersections is the identity on $A$. The whole [Čech cochain complex](../../../../cech-cochain-complex.md) is therefore the same as for the indexed [open cover](../../../../open-cover.md) of a point having the same index set. The [cochain homotopy](../../../../cochain-homotopy.md) constructed in (b) applies component by component and proves

$$
\boxed{\text{Every open subset of }X\text{ is connected},\qquad
\check H^q_{\mathcal U}(X,\underline A)=0\quad(q\geq1).}
$$

The argument concerns the [constant sheaf](../../../../constant-sheaf.md) of [locally constant functions](../../../../locally-constant-function.md); arbitrary coefficient sheaves on an [irreducible topological space](../../../../irreducible-topological-space.md) need not have the same [Čech cohomology](../../../../cech-cohomology.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
