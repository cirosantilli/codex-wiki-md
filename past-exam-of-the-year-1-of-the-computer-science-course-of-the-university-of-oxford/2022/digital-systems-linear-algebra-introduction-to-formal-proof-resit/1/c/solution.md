<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $N$ be the number of nonempty nodes and $d$ the maximum number on a root-to-leaf path. Both listings take **$\Theta(N)$ time** on a unit-cost machine: each node is visited once and its three fields are read once. The recursive listing executes two child calls per nonempty node, including calls on empty children; there are $2N+1$ invocations in total. It saves and restores four words for every nonempty invocation. The iterative listing has one function frame, no recursive calls, and one push/pop pair per deferred nonempty right subtree. Thus it removes repeated call/return and frame-transfer overhead, although its extra loop tests also cost instructions. Exact cycle comparisons need a specified processor, memory timing and compiler; an optimizing compiler may alter either implementation.

For these particular [assembly language](../../../../../assembly-language.md) listings, the recursive [call stack](../../../../../call-stack.md) uses $16d$ bytes above the caller's frame; empty calls allocate no additional frame. The iterative listing uses a fixed $128+16=144$ bytes, even for a shallow or empty tree. With $d\leq32$, the recursive maximum is 512 bytes, versus 144 bytes for this fixed-array iteration. If the promised depth of 32 instead counts edges, the recursive bound is $16\cdot33=528$ bytes; the same 32-word pending array still suffices. Conversely, for $d\leq8$ recursion uses at most 128 bytes and is smaller than the fixed array. When sized dynamically to depth, both approaches use $O(d)$ auxiliary storage, but their stored information differs: full suspended invocation state versus pending subtree roots. Therefore **recursion is not intrinsically always slower or larger**; the claim depends on generated code, tree shape and the choice to reserve a maximum-size explicit array.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
