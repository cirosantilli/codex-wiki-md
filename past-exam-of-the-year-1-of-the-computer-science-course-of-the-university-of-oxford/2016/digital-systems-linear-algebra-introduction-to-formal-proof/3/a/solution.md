<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [calling convention](../../../../../calling-convention.md) passes the integer argument in **`$a0`**, returns the result in **`$v0`**, and uses **`jal` with `$ra`** for a call and its [return address](../../../../../return-address.md). The callee returns using `jr $ra`. Its [stack frame](../../../../../stack-frame.md) grows downwards from `$sp` and must be removed before returning, restoring the caller's [stack pointer](../../../../../stack-pointer.md).

The `$s` [processor registers](../../../../../processor-register.md) are [callee-saved registers](../../../../../callee-saved-register.md): a callee that uses `$s0` or `$s1` must restore their incoming values. The `$a`, `$v`, and `$t` [processor registers](../../../../../processor-register.md) are [caller-saved registers](../../../../../caller-saved-register.md); a caller must preserve any of their values that it needs after a call. Consequently `foo` keeps its own argument in `$s0` and the first call's result in `$s1`, where nested calls preserve them. Because a nested `jal` overwrites `$ra`, `foo` also saves its incoming [return address](../../../../../return-address.md). Every recursive activation has its own [stack frame](../../../../../stack-frame.md).

The supplied [MIPS instructions](../../../../../mips-instruction.md) use the paper's simplified convention: [pseudoinstructions](../../../../../pseudoinstruction.md) such as `subi` are accepted, and control transfers have no [branch delay slot](../../../../../branch-delay-slot.md). The completed code below follows that convention. A hardware implementation with delayed control transfers requires suitable scheduling or `nop` instructions throughout the supplied code as well.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
