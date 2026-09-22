<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [register file](../../../../../register-file.md) with 256 entries needs $\log_2 256=8$ [bits](../../../../../bit.md) per register index. Under the intended assumption that eight times as many instructions are obtained by expanding the primary [opcode](../../../../../opcode.md) field, its width grows from six to $6+\log_2 8=9$ [bits](../../../../../bit.md). Thus **[opcode](../../../../../opcode.md): 9 [bits](../../../../../bit.md); rs, rt and rd: 8 [bits](../../../../../bit.md) each**.

These four fields alone require $9+3(8)=33$ [bits](../../../../../bit.md), already exceeding a 32-[bit](../../../../../bit.md) [instruction encoding](../../../../../instruction-encoding.md). Retaining the five-[bit](../../../../../bit.md) shift amount and six-[bit](../../../../../bit.md) function field of a [MIPS R-type instruction](../../../../../mips-r-type-instruction.md) gives **44 [bits](../../../../../bit.md)**. The processor's data word need not become wider merely because it has more registers.

The [opcode](../../../../../opcode.md) conclusion is conditional: MIPS also uses secondary function fields, so an eightfold increase in the number of semantic operations does not by itself force a nine-[bit](../../../../../bit.md) primary [opcode](../../../../../opcode.md). That is the straightforward field-expansion interpretation of this exercise.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
