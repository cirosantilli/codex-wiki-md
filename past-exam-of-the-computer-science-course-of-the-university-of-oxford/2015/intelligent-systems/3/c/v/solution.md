<h1 id="3/c/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

**Always true for a nonempty finite [constraint domain](../../../../../../constraint-domain.md), as conventionally assumed.** Write $q=|D|$ and identify its values with $\{0,\ldots,q-1\}$. For each satisfying assignment $(x_1,\ldots,x_n)$, simultaneously replace every value by

$$
x_i\longmapsto x_i+a\pmod q,\qquad a\in\{0,\ldots,q-1\}.
$$

This [permutation](../../../../../../permutation.md) of the common [constraint domain](../../../../../../constraint-domain.md) preserves every equality and inequality, hence every [all-different constraint](../../../../../../all-different-constraint.md). The resulting $q$ assignments are distinct: equality of even one coordinate before and after a shift forces $a=0\pmod q$. There is at least one [variable](../../../../../../variable-mathematics.md), since $m>0$ and $k\ge2$.

The [cyclic group](../../../../../../cyclic-group.md) of shifts therefore partitions the solution [set](../../../../../../set-split.md) into disjoint [orbits](../../../../../../orbit-dynamical-system.md) of size $q$. It follows that

$$
\boxed{q\mid\#\operatorname{Sol}(P).}
$$

The conclusion includes an unsatisfiable instance, whose solution count is zero. Full [permutation group](../../../../../../permutation-group.md) orbits need not have size $q!$, because unused values can be permuted without changing an assignment; the cyclic-shift argument avoids that mistake.

If an empty [constraint domain](../../../../../../constraint-domain.md) is permitted, there are zero assignments here, but the wording “divisible by $|D|$” then asks about divisibility by zero, which is ordinarily left undefined. The asserted divisibility uses the standard nonempty-domain convention, and the no-solution conclusion still holds for that degenerate input.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Intelligent systems](../../../../intelligent-systems-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
