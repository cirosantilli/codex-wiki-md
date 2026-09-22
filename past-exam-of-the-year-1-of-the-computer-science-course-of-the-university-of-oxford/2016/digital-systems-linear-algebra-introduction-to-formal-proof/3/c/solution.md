<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The missing [MIPS instructions](../../../../../mips-instruction.md), in order, are
```
bne  $t0, $0, fooRet1
subi $a0, $s0, 3
add  $v0, $s1, $v0
```
The comparison `slti $t0, $s0, 3` makes `$t0` nonzero exactly when $y<3$, so the first instruction selects the base case. The second forms $y-3$ from the saved argument, rather than relying on `$a0` surviving the first call. After the second call, `$s1` holds `bar(y-2)` and `$v0` holds `bar(y-3)`; the final addition puts **their sum in `$v0`**, as required by the [calling convention](../../../../../calling-convention.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
