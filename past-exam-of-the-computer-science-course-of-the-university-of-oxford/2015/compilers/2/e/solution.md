<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Searching the [dynamic chain](../../../../../dynamic-chain.md) would require identifying the procedure associated with each visited [stack frame](../../../../../stack-frame.md). More seriously, the search length is bounded by the number $h$ of active calls, not by lexical nesting depth. Recursion in procedures unrelated to the desired enclosing declaration can make $h$ arbitrarily large. Thus a single [nonlocal variable](../../../../../nonlocal-variable.md) access can take $O(h)$ [time complexity](../../../../../time-complexity.md), whereas a conventional [static chain](../../../../../static-chain.md) access needs only $d$ traversals for lexical distance $d$.

Instead give each procedure $P$ a known global [pointer](../../../../../pointer-computer-programming.md) cell `current[P]`. On entry to $P$, save its previous value in the new [stack frame](../../../../../stack-frame.md) and set `current[P]` to the new [frame pointer](../../../../../frame-pointer.md). On return, restore the saved value. A [nonlocal variable](../../../../../nonlocal-variable.md) declared in $P$ is then loaded using `current[P]` and its known frame offset. The proof in part (d) justifies that lookup in the absence of [procedural parameters](../../../../../procedural-parameter.md). This is a procedure-indexed version of a [display for lexical scope](../../../../../display-for-lexical-scope.md); a conventional [display for lexical scope](../../../../../display-for-lexical-scope.md) can instead use lexical levels as indices.

With $m$ procedures and $h$ active calls, the procedure-indexed table needs $O(m)$ additional global words and one saved previous [pointer](../../../../../pointer-computer-programming.md) per active [stack frame](../../../../../stack-frame.md), hence $O(h)$ activation storage. The saved word can replace the conventional per-frame [static link](../../../../../static-link.md) if that link is no longer needed. A conventional [static chain](../../../../../static-chain.md) has one [pointer](../../../../../pointer-computer-programming.md) per active [stack frame](../../../../../stack-frame.md) and no such $m$-entry table. Both schemes retain ordinary [dynamic links](../../../../../dynamic-link.md) and return information.

The table gives **constant-time nonlocal access and constant-time save/restore work on each entry/return**, independently of lexical distance. Conventional [static chain](../../../../../static-chain.md) access costs $O(d)$ per access, and establishing the callee's [static link](../../../../../static-link.md) may also require following an appropriate portion of the caller's chain. For a fixed program $d$ is statically bounded, but it still affects generated instruction counts. These costs assume constant-cost [pointer](../../../../../pointer-computer-programming.md) operations and omit shared ordinary call overhead. For the procedure-indexed table,

$$
\boxed{T_{\mathrm{access}}=O(1),\quad T_{\mathrm{entry/return}}=O(1),\quad S_{\mathrm{environment}}=O(m+h).}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Compilers](../../../compilers-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
