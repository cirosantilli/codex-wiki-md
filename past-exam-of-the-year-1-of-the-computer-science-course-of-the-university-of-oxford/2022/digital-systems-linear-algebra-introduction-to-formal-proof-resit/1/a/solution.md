<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use `r0` for the argument and result. With 32-bit [integers](../../../../../integer-split.md) and [pointers](../../../../../pointer-computer-programming.md), the three fields have byte offsets 0, 4 and 8. Assume an acyclic finite [binary tree](../../../../../binary-tree.md), no concurrent mutation, a valid aligned [call stack](../../../../../call-stack.md), and no signed [integer overflow](../../../../../integer-overflow.md) in any evaluated sum. These are representation and arithmetic assumptions, rather than properties of arbitrary [C programming language](../../../../../c-programming-language.md) implementations.

```
.syntax unified
.cpu cortex-m0
.thumb
.global sum_rec
.thumb_func
sum_rec:
    cmp  r0, #0
    beq  .Lempty
    push {r4, r5, r6, lr}    @ 16-byte frame; r6 is alignment padding
    movs r4, r0              @ retain this invocation's node
    ldr  r5, [r4, #0]        @ running value begins with its label
    ldr  r0, [r4, #4]
    bl   sum_rec             @ r0 = left subtree sum
    adds r5, r5, r0
    ldr  r0, [r4, #8]
    bl   sum_rec             @ r0 = right subtree sum
    adds r0, r0, r5
    pop  {r4, r5, r6, pc}    @ restore caller state and return
.Lempty:
    movs r0, #0
    bx   lr
```

The node and partial sum are held in [callee-saved registers](../../../../../callee-saved-register.md) `r4,r5`. Each recursive invocation saves its caller's values before replacing them, so a child returns with the parent's values intact. Saving `lr` preserves the return address across the two `bl` instructions. [Caller-saved registers](../../../../../caller-saved-register.md) may be overwritten by a child; no parent value is left live only in them. Pushing four words maintains eight-byte [stack alignment](../../../../../stack-alignment.md) at recursive calls.[AAPCS32, base standard: core-register roles, stack constraints and result return](../../../../../procedure-call-standard-for-the-arm-architecture-by-arm-limited.md)

Correctness follows by [structural induction](../../../../../structural-induction.md). An empty subtree returns zero. For a nonempty subtree, assume both recursive calls return their respective label sums. The final addition then combines the node's label with exactly those two sums, so **`r0` returns the sum of all labels**. The instruction forms and field offsets fit the short load and arithmetic encodings.[Move, Add, Load, Push/Pop and Branch tables](../../../../../thumb-16-bit-instruction-set-quick-reference-by-arm.md)

## ↑ Ancestors (12)

1. [A](../a.md)
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
