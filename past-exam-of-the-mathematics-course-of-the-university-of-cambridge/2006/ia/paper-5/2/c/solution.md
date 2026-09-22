<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**True.** In [polled input-output](../../../../../../polled-input-output.md), a processor reads device status and handles ready work without [interrupt](../../../../../../interrupt.md) entry and return overhead. If an operation completes very quickly, or requests arrive continuously at a high rate, a short poll or a batch of polls can cost less than an [interrupt](../../../../../../interrupt.md) for every event. [Interrupt-driven input-output](../../../../../../interrupt-driven-input-output.md) is usually better for long or infrequent waits because the processor can do unrelated work or sleep instead of busy waiting. The useful choice depends on the event rate and latency requirement.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
