<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The entry sequence creates one 12-byte [stack frame](../../../../../stack-frame.md), then preserves the [return address](../../../../../return-address.md) and both used [callee-saved registers](../../../../../callee-saved-register.md):
```
subi $sp, $sp, 12    # allocate three four-byte words
sw   $ra, 0($sp)     # save return address of this activation
sw   $s0, 4($sp)     # save caller's s0
sw   $s1, 8($sp)     # save caller's s1
```
The closing sequence reverses these effects:
```
lw   $ra, 0($sp)     # recover return address of this activation
lw   $s0, 4($sp)     # restore caller's s0
lw   $s1, 8($sp)     # restore caller's s1
addi $sp, $sp, 12    # deallocate the frame
jr   $ra            # return to the caller
```
Loads must precede deallocation because their offsets refer to the current [stack frame](../../../../../stack-frame.md). The [return value](../../../../../return-value.md) in `$v0` is deliberately retained. Saving `$ra` is essential even though it is not an `$s` [processor register](../../../../../processor-register.md): otherwise the second nested call would destroy the address to which this activation must return.

## ↑ Ancestors (12)

1. [B](../b.md)
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
