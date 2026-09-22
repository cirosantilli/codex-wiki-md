<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\kappa=|\alpha|$ be the infinite [initial ordinal](../../../../../initial-ordinal.md) of the given [ordinal](../../../../../ordinal-split.md). A successor adds only one point, so $|\alpha+1|=\kappa$: one can absorb the additional point by shifting the initial copy of $\omega$ and fixing the rest.

The successor construction from part (a) partitions the new range into the old range, a new row of size $|\alpha+1|$, and a new column of size $|\alpha|$. By hypothesis each part has [cardinality](../../../../../cardinality.md) at most $\kappa$, and the old range already has [cardinality](../../../../../cardinality.md) $\kappa$.

A finite [disjoint union](../../../../../disjoint-union.md) of copies of a well-orderable infinite cardinal has that same [cardinality](../../../../../cardinality.md) without invoking the square theorem being proved. Explicitly, write each $\xi<\kappa$ uniquely as $\omega\eta+n$ with $n<\omega$. Interleave three copies by

$$
(\xi,j)\longmapsto\omega\eta+3n+j,\qquad j<3.
$$

This stays below $\kappa$ because an infinite [initial ordinal](../../../../../initial-ordinal.md) is a limit [ordinal](../../../../../ordinal-split.md) and is closed under finite successor steps below it. It is [injective](../../../../../injective-function.md) by uniqueness of the quotient and finite remainder. The reverse [injection](../../../../../injective-function.md) is immediate, so the [Cantor-Schröder-Bernstein theorem](../../../../../cantor-schroder-bernstein-theorem.md) proves the finite-union claim.

Applying that bound to the three range pieces yields

$$
\boxed{|\gamma_{\alpha+1}|=\kappa=|\alpha+1|.}
$$

Only the well-orderability of [ordinals](../../../../../ordinal-split.md), not a choice principle for arbitrary families of sets, was used.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
