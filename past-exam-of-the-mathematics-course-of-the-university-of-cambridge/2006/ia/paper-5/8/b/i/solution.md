<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Add profiling to the timer-[interrupt](../../../../../../../interrupt.md) handler. When the target [operating-system process](../../../../../../../process-computing.md) is interrupted while running, record its saved [instruction pointer](../../../../../../../instruction-pointer.md), map that address to a code region in the executable, and increment an address histogram. Addresses with many samples identify regions consuming a large fraction of execution time. The executable's code can then be disassembled around these addresses even when source and symbolic names are absent.

This is [statistical program profiling](../../../../../../../statistical-program-profiling.md): uniform samples of running time estimate time spent in code, not exact execution counts. Restrict samples to the desired process and distinguish application execution from unrelated kernel work. A sufficiently fine address histogram and many samples reveal hot loops; varying the sample interval reduces synchronization bias. If exact visit counts rather than time hotspots are needed, arrange breakpoint or single-step traps, or rewrite the binary to add counters, accepting their much larger overhead. **Source code is not required to associate sampled execution with instruction addresses.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
