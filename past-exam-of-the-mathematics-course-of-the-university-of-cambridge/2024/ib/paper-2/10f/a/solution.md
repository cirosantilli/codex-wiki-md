<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A topological space is compact if every open cover has a finite subcover. It is Hausdorff if every pair of distinct points has disjoint open neighbourhoods.

Let $Y$ be closed in compact $X$, and let $\{U_i\}$ be an open cover of $Y$ by sets open in $X$. Adding the [open set](../../../../../../open-set.md) $X\setminus Y$ gives a cover of $X$, which has a finite subcover. Removing $X\setminus Y$ leaves a finite subcover of $Y$. Thus every closed subspace of a [compact space](../../../../../../compact-space.md) is compact.

Now let $A,B$ be disjoint closed subsets of a compact Hausdorff space. They are compact. For each $a\in A$ and $b\in B$, choose disjoint [open sets](../../../../../../open-set.md) $U_{a,b}\ni a$ and $V_{a,b}\ni b$. Fixing $a$, finitely many $V_{a,b_j}$ cover $B$. Put

$$
U_a=\bigcap_jU_{a,b_j},
\qquad
V_a=\bigcup_jV_{a,b_j}.
$$

Then $U_a$ contains $a$, $V_a$ contains $B$, and they are disjoint. Finitely many $U_{a_i}$ cover $A$. Therefore

$$
U=\bigcup_iU_{a_i},
\qquad
V=\bigcap_iV_{a_i}
$$

are disjoint open neighbourhoods of $A$ and $B$. This proves the [normality of a compact Hausdorff space](../../../../../../normality-of-a-compact-hausdorff-space.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
