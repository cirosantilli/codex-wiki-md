<h1 id="8/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The processor selects the device's data or control register by presenting its address, either in memory-mapped input-output space or in a distinct port-address space. For a write, it places data on the [computer bus](../../../../../../../computer-bus.md) and asserts the appropriate write control. For a read, it asserts read control and samples the data supplied by the addressed device. The device recognizes the address and uses the bus timing or acknowledge protocol to indicate completion, including wait states if needed.

The processor uses status registers to determine readiness and control registers to request operations. This register-level communication can be arranged using [polled input-output](../../../../../../../polled-input-output.md) or [interrupt-driven input-output](../../../../../../../interrupt-driven-input-output.md); the bus transaction itself and the policy for waiting on a device are separate issues.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
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
