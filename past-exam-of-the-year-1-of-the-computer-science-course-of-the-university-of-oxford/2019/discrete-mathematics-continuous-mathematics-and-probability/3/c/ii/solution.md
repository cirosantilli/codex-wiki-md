<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The displayed relation is not a [partial order](../../../../../../partially-ordered-set.md) on the printed $A$.** Since the [empty set](../../../../../../empty-set.md) belongs to $A$, [vacuous truth](../../../../../../vacuous-truth.md) makes

$$
\varnothing\preceq_2 T,\qquad T\preceq_2\varnothing
$$

hold for every finite $T$, including nonempty $T$. This violates the defining condition of an [antisymmetric relation](../../../../../../antisymmetric-relation.md). It also violates [transitivity](../../../../../../transitive-relation.md): $\{2\}\preceq_2\varnothing\preceq_2\{1\}$ holds, but $\{2\}\npreceq_2\{1\}$. Consequently the usual unique-maximum and unique-[least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) terminology for a [partially ordered set](../../../../../../partially-ordered-set.md) does not apply as claimed.

The available inputs still determine what happens if one applies the formulas in (b) literally to this relation:

| Family | Elements satisfying the maximum formula | Elements satisfying the least-upper-bound formula |
| --- | --- | --- |
| $S_1$ | None | $\varnothing$ |
| $S_2$ | $\varnothing$ and $\{100\}$ | $\varnothing$ and $\{100\}$ |
| $S_1\cap S_2$ | None | $\varnothing$ and $\{100\}$ |

For $S_1$, no nonempty finite [set](../../../../../../set-split.md) can lie above all triples of arbitrarily large numbers, while $\varnothing$ does so vacuously. Thus $\varnothing$ is its sole literal [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md), but is not a member of $S_1$. For each of the two bounded families, the literal [upper bounds](../../../../../../upper-bound-in-a-partially-ordered-set.md) are $\varnothing$ and all nonempty finite [sets](../../../../../../set-split.md) whose elements are at least $100$. Among these, exactly $\varnothing$ and $\{100\}$ lie below every such [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md). Both belong to $S_2$, but neither belongs to its three-element subfamily.

For comparison, a natural correction is to retain the given rule for nonempty [sets](../../../../../../set-split.md) and declare $\varnothing$ to be a bottom element: no nonempty [set](../../../../../../set-split.md) is then below $\varnothing$. Under this explicitly corrected [partial order](../../../../../../partially-ordered-set.md), **$S_1$ has neither a maximum nor a [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md); $S_2$ has maximum and [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) $\{100\}$; and $S_1\cap S_2$ has no maximum but has [least upper bound](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) $\{100\}$.** A nonempty [upper bound](../../../../../../upper-bound-in-a-partially-ordered-set.md) must have every element at least as large as every element of the bounded family. These corrected answers are conditional on the stated repair, not answers obtained by silently excluding the [empty set](../../../../../../empty-set.md) from the source.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
