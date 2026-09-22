<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Removing [logic hazards](../../../../../hazard-logic.md) prevents transient false control pulses, incorrect triggering of asynchronous state changes and avoidable switching activity. It also makes behavior less sensitive to unequal [propagation delays](../../../../../propagation-delay.md). These benefits matter especially when an output directly controls another circuit rather than being sampled only after settling.

The usual costs are redundant [logic gates](../../../../../logic-gate.md), larger area and capacitance, more wiring and possibly a longer [critical path](../../../../../combinational-critical-path.md). Power can rise from extra hardware even when glitch power falls. A synchronous design may instead sample after a sufficiently long clock period, trading settling time against additional hazard-correction logic. A circuit proved free of single-input static hazards need not be safe under arbitrary simultaneous input changes; [metastability](../../../../../metastability.md) at an asynchronous input is a different problem.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
