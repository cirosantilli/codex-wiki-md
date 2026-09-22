<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Run the following two [MIPS instruction](../../../../../../mips-instruction.md) tests separately from externally prepared states, and inspect the [register file](../../../../../../register-file.md) after the indicated instruction. External preparation is useful in a manufacturing test: code that initializes [processor registers](../../../../../../processor-register.md) through the very control line being tested need not work. Assume the one potentially faulty line is `RegDst`; all other lines work normally.

For the first test, preset `$t0=7`, `$t1=5`, `$t2=99`, and execute
```
add $t2, $t0, $t1
```
The encoded `rt` is `$t1`, while `rd` is `$t2`. A healthy line or a line stuck at one writes 12 into `$t2`. A line stuck at zero instead writes 12 into `$t1`, leaving `$t2=99`.

For the second test, preset `$t3=4`, `$s0=L`, and the aligned memory word at $L$ to 37, then execute
```
lw $t3, 0($s0)
```
The zero immediate makes instruction bits $15\ldots11$ zero. A healthy line or a line stuck at zero writes 37 into `$t3`; a line stuck at one attempts to write the [MIPS zero register](../../../../../../mips-zero-register.md), leaving `$t3=4`. The [MIPS zero register](../../../../../../mips-zero-register.md) ignores attempted writes. Thus, recording the first test's `$t2` and the second test's `$t3`,

$$
\boxed{\begin{array}{c|c}
\text{RegDst state}&(t2,t3)\\\hline
\text{normal}&(12,37)\\
\text{stuck at 0}&(99,37)\\
\text{stuck at 1}&(12,4)
\end{array}}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
