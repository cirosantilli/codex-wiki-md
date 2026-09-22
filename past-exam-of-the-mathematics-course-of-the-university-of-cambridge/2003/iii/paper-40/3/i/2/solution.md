<h1 id="3/i/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A classical [sequential probability ratio test](../../../../../../../sequential-probability-ratio-test.md) addresses a fixed-start choice between two simple [statistical hypotheses](../../../../../../../statistical-hypothesis.md). It sums [log-likelihood ratio](../../../../../../../log-likelihood-ratio.md) increments until an upper boundary accepts the alternative or a lower boundary accepts the null; it then terminates that test. A [CUSUM](../../../../../../../cusum.md) instead monitors indefinitely for a change at an unknown time. Its reset at zero discards sustained evidence from a previously satisfactory period, so a late change need not first undo all earlier negative scores. An upper boundary $h$ signals when the accumulated change evidence is sufficiently large.

A [fast initial response CUSUM](../../../../../../../fast-initial-response-cusum.md) takes $0<X_0<h$, often $X_0=h/2$, in place of a zero start. Until its first reset or signal, it acts like a fixed-start [sequential probability ratio test](../../../../../../../sequential-probability-ratio-test.md) with a lower boundary at $-X_0$ and an upper boundary at $h-X_0$ for the subsequent cumulative increments. Upon reaching the lower boundary it resets and continues as an ordinary [CUSUM](../../../../../../../cusum.md). **The head start gives faster detection if a change is already present when monitoring begins or restarts.** It is useful after an intervention, a shutdown or a previous alarm when immediate renewed surveillance is desired. Its initial false-alarm behavior differs from the zero-start scheme, so the head start and signalling boundary must be calibrated together; the preceding numerical choice is a design convention, not a universal optimum.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [I](../../i.md)
3. [3](../../../3.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
