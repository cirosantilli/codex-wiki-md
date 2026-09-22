<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an estimate, use the usual equal-device [CMOS](../../../../../cmos.md) series-stack model: a $k$-input [NAND gate](../../../../../nand-gate.md) or [NOR gate](../../../../../nor-gate.md) has a worst-case [propagation delay](../../../../../propagation-delay.md) approximately $k$ times that of an inverter, because a conducting path contains $k$ series [transistors](../../../../../transistor.md). An [AND gate](../../../../../and-gate.md) or [OR gate](../../../../../or-gate.md) adds an output inverter. With a 1 ns inverter this gives, for $k\geq2$,

$$
\boxed{t_{\mathrm{AND},k}\simeq t_{\mathrm{OR},k}\simeq(k+1)\,\mathrm{ns}.}
$$

For $k=2$ it reproduces the stated 3 ns. This is a technology estimate under equal sizing and comparable loading, not a unique physical law inferable from a single measured delay. Actual [propagation delay](../../../../../propagation-delay.md) also depends on [capacitance](../../../../../capacitance.md), [fan-out](../../../../../fan-out.md) and [transistor](../../../../../transistor.md) sizing. If instead only the supplied two-input gates were allowed, a balanced tree would have worst-case depth $\lceil\log_2k\rceil$ and delay $3\lceil\log_2k\rceil$ ns; that is a different construction from a single $k$-input gate.

For the explicit circuit in part (a), the longest [combinational logic](../../../../../combinational-logic.md) path starts at $A$, passes through the shared inverter, either direction-match [exclusive or](../../../../../exclusive-or.md), the [AND gate](../../../../../and-gate.md), and the final [exclusive or](../../../../../exclusive-or.md) feeding $D_2$:

$$
\boxed{t_{\max}=1+2+3+2=8\,\mathrm{ns}.}
$$

The path $A\to D_1$ takes 5 ns, the paths from $B0$ or $B1$ to $D_2$ take at most 7 ns, and $B0\to D_0$ takes 1 ns. Both direction-match [exclusive or](../../../../../exclusive-or.md) gates act in parallel; their delays are not added together. The 8 ns excludes [clock-to-Q delay](../../../../../clock-to-q-delay.md), [setup time](../../../../../setup-time.md), [hold time](../../../../../hold-time.md) and clock-distribution effects, because the question asks only for the [combinational logic](../../../../../combinational-logic.md) delay.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
