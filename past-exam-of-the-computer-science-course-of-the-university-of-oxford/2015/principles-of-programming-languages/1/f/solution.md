<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Expand the two [type synonyms](../../../../../type-synonym.md) to see what survives an exception:

$$
\begin{aligned}
\operatorname{ExT}(\operatorname{MemT}\ m)\ A
&=\operatorname{Mem}\to m(\operatorname{Maybe}\ A,\operatorname{Mem}),\\
\operatorname{MemT}(\operatorname{ExT}\ m)\ A
&=\operatorname{Mem}\to m(\operatorname{Maybe}(A,\operatorname{Mem})).
\end{aligned}
$$

In the first order, a failed computation can still produce `(Nothing,s')`. The exception handler therefore runs with $s'$, including writes made before failure. In the second order, failure produces `Nothing`, with no returned [computer memory](../../../../../computer-memory-split.md). A handler defined by applying the underlying `orelse` pointwise runs its alternative from the original input [computer memory](../../../../../computer-memory-split.md) $s$. This gives rollback of this explicit [program state](../../../../../program-state.md) for the failed branch.

For example, start with a [memory location](../../../../../memory-location.md) holding $0$, write $1$, fail, and handle the failure by reading that [memory location](../../../../../memory-location.md). The first order returns $1$; the second returns $0$. This rollback concerns the explicit [computer memory](../../../../../computer-memory-split.md) only: arbitrary effects in the base [computational monad](../../../../../computational-monad.md) are not thereby reversed.

$$
\boxed{\begin{aligned}
\operatorname{ExT}(\operatorname{MemT}\ m)&:\text{ writes survive failure};\\
\operatorname{MemT}(\operatorname{ExT}\ m)&:\text{ failed memory updates roll back}.
\end{aligned}}
$$

A conventional [programming language](../../../../../programming-language-split.md) normally retains writes made before an exception is caught. Its mutable [computer memory](../../../../../computer-memory-split.md) and [exception handling](../../../../../exception-handling.md) therefore correspond more closely to $\operatorname{ExT}(\operatorname{MemT}\ m)$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Principles of programming languages](../../../principles-of-programming-languages-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
