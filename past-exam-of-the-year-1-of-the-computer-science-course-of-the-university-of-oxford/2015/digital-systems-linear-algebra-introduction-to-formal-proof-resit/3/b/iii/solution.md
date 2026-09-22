<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Again use independent externally initialized [MIPS instruction](../../../../../../mips-instruction.md) tests. First preset `$t0=7`, `$t1=5`, and execute
```
add $t2, $t0, $t1
```
The normal result, also obtained with `ALUSrc` stuck at zero, is 12. If the line is stuck at one, the second [ALU](../../../../../../arithmetic-logic-unit.md) operand is the sign-extended low 16 instruction [bits](../../../../../../bit.md). For this exact instruction they encode `rd=10`, shift amount zero and function $\mathtt{0x20}$, giving $\mathtt{0x5020}=20512$. The erroneous result is therefore $7+20512=20519$.

For the second test, preset `$s0=L`, `$t3=4`, memory at $L$ to 37 and memory at $L+4$ to 99, with both words valid and aligned. Execute
```
lw $t3, 0($s0)
```
Normally, and with `ALUSrc` stuck at one, the address is $L+0$ and the result is 37. With the line stuck at zero, the second [ALU](../../../../../../arithmetic-logic-unit.md) operand is the old `$t3=4`, so the load reads 99 from $L+4$. Thus

$$
\boxed{\begin{array}{c|c}
\text{ALUSrc state}&(t2\text{ after add},t3\text{ after load})\\\hline
\text{normal}&(12,37)\\
\text{stuck at 0}&(12,99)\\
\text{stuck at 1}&(20519,37)
\end{array}}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
