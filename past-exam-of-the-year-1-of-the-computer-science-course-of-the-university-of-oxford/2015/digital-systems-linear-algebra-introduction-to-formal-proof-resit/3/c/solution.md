<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [register file](../../../../../register-file.md) in this [datapath](../../../../../datapath.md) supplies both read ports combinationally for whatever read addresses the instruction fields present. Reading a [processor register](../../../../../processor-register.md) is harmless, and a result that the current [MIPS instruction](../../../../../mips-instruction.md) does not need can simply be ignored. Only writes require an explicit enable because writes change architectural state. There is consequently no functional need for `RegRead` in this design.

The data-memory read interface has an explicit `MemRead` enable. Non-load [MIPS instructions](../../../../../mips-instruction.md) can present irrelevant or invalid addresses at the memory address input; an external memory transaction should not be initiated merely because those [bits](../../../../../bit.md) happen to be present. An explicit enable also permits interfaces with [memory-mapped input-output](../../../../../memory-mapped-input-output.md), where a read can have a side effect. It can reduce unnecessary activity even for ordinary memory.

$$
\boxed{\text{register reads are continuously available; memory reads are explicitly requested.}}
$$

This is a distinction in the supplied [datapath](../../../../../datapath.md), rather than a universal physical prohibition: other [register files](../../../../../register-file.md) can have read enables, and an ideal side-effect-free memory can be modeled with continuous reads.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
