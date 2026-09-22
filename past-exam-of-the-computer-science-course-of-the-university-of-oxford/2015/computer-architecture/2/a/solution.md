<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the illustrated [out-of-order execution](../../../../../out-of-order-execution.md) scheme without a [reorder buffer](../../../../../reorder-buffer.md), a [reservation station](../../../../../reservation-station.md) identifier acts as the producer tag for an outstanding result. A [register renaming](../../../../../register-renaming.md) map and waiting operands in other [reservation stations](../../../../../reservation-station.md) can refer to that tag. The tag must remain unique until the result has been broadcast and the required [register file](../../../../../register-file.md) update has occurred.

For example, issue a slow multiplication producing `r1` into [reservation station](../../../../../reservation-station.md) S, then an addition `r4 := r1 + r5` into another [reservation station](../../../../../reservation-station.md). The addition records S as the unresolved source of `r1`. Even after the multiplier has accepted its operands, the multiplication can take many cycles; S cannot be reassigned merely because its operands have left the [reservation station](../../../../../reservation-station.md). If an independent short instruction is assigned S and broadcasts first, the addition would mistake that unrelated value for the multiplication's result. A later multiplication result could likewise corrupt the new instruction's [register renaming](../../../../../register-renaming.md) mapping.

Finishing execution is also insufficient if the result is waiting for [common data bus](../../../../../common-data-bus.md) access: consumers and the [register file](../../../../../register-file.md) still name S until writeback. **Keep the producer tag allocated through broadcast/writeback, so no younger result can masquerade as the outstanding producer.** With a separate persistent producer tag, such as a [reorder buffer](../../../../../reorder-buffer.md) entry or a [physical register](../../../../../physical-register.md), a design can release the scheduling slot earlier; this changes the tag-ownership arrangement in the question.

$$
\boxed{\text{Do not reuse a producer tag before its result has been broadcast.}}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
