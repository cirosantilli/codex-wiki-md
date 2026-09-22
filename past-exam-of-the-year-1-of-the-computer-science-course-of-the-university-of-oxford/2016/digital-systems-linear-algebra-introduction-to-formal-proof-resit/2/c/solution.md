<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Address a [read-only memory](../../../../../read-only-memory.md) with the two state [bits](../../../../../bit.md) and two input [bits](../../../../../bit.md). Each word stores the two next-state bits and `INC`, so a direct replacement for all the combinational logic is **$16\times3$ bits, or 48 bits**. Program its 16 words from the state table, duplicating a state's output over all four input addresses. The two [D flip-flops](../../../../../d-flip-flop.md) and clock remain outside the ROM.

If `INC` retains its separate two-state-bit decoder, only the next-state logic needs a **$16\times2$-bit ROM**, plus that output gate. Storing output in a separate state-only ROM would use $4\times1$ further bits. These factored options have a different boundary from replacing all the combinational logic with one ROM.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
