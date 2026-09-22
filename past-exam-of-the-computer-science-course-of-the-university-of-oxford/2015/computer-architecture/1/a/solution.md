<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Register forwarding](../../../../../register-forwarding.md) supplies a later instruction with a computed value before that value has reached the [register file](../../../../../register-file.md). It removes some [read-after-write hazards](../../../../../read-after-write-hazard.md) without changing the program's meaning. Consider these symbolic [machine instructions](../../../../../machine-instruction.md), with the destination first:
```
ADD r1, r2, r3
SUB r4, r1, r5
```
In the five-stage [in-order pipeline](../../../../../in-order-pipeline.md), the addition produces its result at the end of EX. In the next cycle the subtraction is in EX, although the addition has not yet reached WB. A bypass from the addition's EX/MEM [pipeline register](../../../../../pipeline-register.md) to the subtraction's [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) input supplies the new `r1`; the old value read in ID must be overridden.

The bypass control compares source and destination [processor register](../../../../../processor-register.md) identifiers and selects the youngest applicable older producer. It must also check that the producer actually writes that [processor register](../../../../../processor-register.md). **Forward the newest available result instead of waiting for its writeback.** A [load instruction](../../../../../load-instruction.md) is different: its value is normally available only at the end of MEM, so an immediately following dependent instruction still needs a [pipeline stall](../../../../../pipeline-stall.md) in this five-stage arrangement.

$$
\boxed{\text{Forward the newest ready result directly to its dependent instruction.}}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Computer architecture](../../../computer-architecture-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
