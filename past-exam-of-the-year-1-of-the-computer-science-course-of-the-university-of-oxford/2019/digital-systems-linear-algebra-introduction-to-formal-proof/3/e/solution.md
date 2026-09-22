<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The likely effect in a single-cycle or unchanged pipeline-stage implementation is a **longer [combinational critical path](../../../../../combinational-critical-path.md) and hence a lower maximum [processor clock frequency](../../../../../processor-clock-frequency.md)**. Previously the [barrel shifter](../../../../../barrel-shifter.md) and [ALU](../../../../../arithmetic-logic-unit.md) could work in parallel before result selection; the modified path can require both shift and addition before address or result use.

Ignoring common [processor register](../../../../../processor-register.md) and wiring delays, the relevant [combinational logic](../../../../../combinational-logic.md) contribution changes roughly from $\max(t_{\mathrm{ALU}},t_{\mathrm{shift}})+t_{\mathrm{mux}}$ to $t_{\mathrm{shift}}+t_{\mathrm{ALU}}$, with any additional input selection included as needed. The [processor clock period](../../../../../processor-clock-period.md) must also cover [processor register](../../../../../processor-register.md) timing and the rest of the instruction path, potentially including memory access. Removing a [multiplexer](../../../../../multiplexer.md) offsets some delay, so a numerical frequency change cannot be inferred without component timings. Pipelining, a faster implementation or another pre-existing bottleneck can alter the outcome; the changed serial dependence is the reason for the likely reduction.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
