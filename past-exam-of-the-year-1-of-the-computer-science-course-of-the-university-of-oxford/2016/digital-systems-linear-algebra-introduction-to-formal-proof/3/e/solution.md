<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Keep both the limit and current argument in [callee-saved registers](../../../../../callee-saved-register.md), so a call to `foo` preserves them. Under the same no-delay-slot convention, use
```
li   $s0, n
li   $s1, 1
slti $t0, $s0, 1
bne  $t0, $0, testEnd
testLoop:
move $a0, $s1
jal  foo
break 1
beq  $s1, $s0, testEnd
addi $s1, $s1, 1
b    testLoop
testEnd:
break 0
b    testEnd
```
At every **`break 1`**, `$s1` is the tested value and `$v0` is its result. Resuming after the breakpoint continues to the next value; after $n$ the program reaches its separate final stop. The initial guard handles $n<1$ with no calls. Testing equality before incrementing also avoids overflowing the loop variable after the final call when $n$ is the largest positive machine integer. As with the supplied procedures, evaluating all calls assumes enough [stack](../../../../../stack-data-structure.md) space and representable arithmetic results.

## ↑ Ancestors (12)

1. [E](../e.md)
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
