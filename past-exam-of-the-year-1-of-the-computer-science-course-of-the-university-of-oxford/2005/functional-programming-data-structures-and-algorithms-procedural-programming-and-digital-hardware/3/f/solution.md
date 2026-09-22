<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

On two finite total [lists](../../../../../list-abstract-data-type.md), the equations agree. If either [list](../../../../../list-abstract-data-type.md) is empty they return the other; if both have heads, expanding `twiddle` twice gives `x : y : twiddle xs ys`, exactly the third equation for `twiddle'`. The same finite-prefix reasoning proves agreement on infinite inputs with defined spines.

They differ on [partial lists](../../../../../partial-list.md). Take the first argument `[1]` and the second argument $\bot$. The original definition can emit its first head immediately:

$$
\operatorname{twiddle}\ [1]\ \bot
=1:\operatorname{twiddle}\ \bot\ []
=1:\bot.
$$

After recognizing the nonempty first argument, `twiddle'` must inspect the second argument to distinguish its second and third equations. That inspection diverges, so

$$
\operatorname{twiddle}'\ [1]\ \bot=\bot,\qquad
\boxed{\operatorname{twiddle}'\ne\operatorname{twiddle}.}
$$

For example, demanding only the head distinguishes them: the original returns `1`, while the primed version diverges. Equality of [functions](../../../../../function-split.md) under [lazy evaluation](../../../../../lazy-evaluation.md) requires agreement on these partial inputs too.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
