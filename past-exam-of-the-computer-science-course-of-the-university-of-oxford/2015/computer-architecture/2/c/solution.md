<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Consider a slow [load instruction](../../../../../load-instruction.md) controlling one conditional addition, followed by independent work. The following is schematic A32 [assembly language](../../../../../assembly-language.md); the plain `ADD` and `MUL` forms shown do not update [processor condition flags](../../../../../processor-condition-flag.md):
```
LDR r0, [r1]
CMP r0, #0
BNE skip
ADD r2, r2, #1
skip:
MUL r8, r9, r10
```
Without [branch prediction](../../../../../branch-prediction.md), the unresolved conditional branch prevents fetching beyond it until the [load instruction](../../../../../load-instruction.md), comparison and branch resolution complete. The multiplication does not depend on `r0`, yet the [out-of-order execution](../../../../../out-of-order-execution.md) machinery cannot execute it if it has not been fetched and issued.

[Conditional execution](../../../../../conditional-execution.md) removes that branch:
```
LDR   r0, [r1]
CMP   r0, #0
ADDEQ r2, r2, #1
MUL   r8, r9, r10
```
`ADDEQ` adds one exactly when the [zero flag](../../../../../zero-flag.md) from `CMP` is set; otherwise it preserves `r2`. The instruction stream has a known sequential continuation, so the [CPU](../../../../../central-processing-unit.md) can fetch and issue the multiplication while the [load instruction](../../../../../load-instruction.md) is outstanding. With available [reservation stations](../../../../../reservation-station.md) and a free multiplier, independent multiplication overlaps the [load instruction](../../../../../load-instruction.md)'s [latency](../../../../../latency-engineering.md).

**Predication removes a control-flow obstacle to finding independent work; it does not resolve the slow load or its dependent condition earlier.** The conditional addition must still select the correct result after the [processor condition flags](../../../../../processor-condition-flag.md) become known. The gain is especially useful for a short conditional region, since instructions whose predicates are false still occupy fetch and issue resources. On a strictly blocking [in-order pipeline](../../../../../in-order-pipeline.md), a slow demand [load instruction](../../../../../load-instruction.md) would still stop later work in MEM; the overlap here uses the question's [out-of-order execution](../../../../../out-of-order-execution.md) setting and a nonblocking memory path.

$$
\boxed{\text{Predication exposes independent later work while the condition waits.}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Computer architecture](../../../computer-architecture-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
