<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Move the no-write decision into the destination-address path. If the original destination selection produced $d$ and the original write-enable decision was $W$, drive the new register file with

$$
\boxed{\mathrm{wa}=\begin{cases}d,&W=1,\\0,&W=0.\end{cases}}
$$

A five-bit two-input [multiplexer](../../../../../../multiplexer.md) after the existing destination selector implements this, or the decoder can directly select among zero, the instruction's destination fields and register 31. Its control still distinguishes writing and non-writing instructions: removing the register-file enable pin does not remove that logical decision.

Read-address selection and the result-data path can remain unchanged. Instructions that formerly disabled RegWrite now select destination zero; their write data is irrelevant. Instructions writing an actual destination preserve the same address and data. Since writes to the [MIPS zero register](../../../../../../mips-zero-register.md) were already discarded, the architectural behaviour is unchanged for that case as well.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
