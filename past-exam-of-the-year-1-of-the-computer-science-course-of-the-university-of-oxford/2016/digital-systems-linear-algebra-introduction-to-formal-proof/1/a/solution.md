<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a synchronous [binary counter](../../../../../binary-counter.md) with three positive-edge-triggered [D flip-flops](../../../../../d-flip-flop.md), all driven by the same [clock signal](../../../../../clock-signal.md). Write their outputs $q_2q_1q_0$, with $q_0$ the [least significant bit](../../../../../least-significant-bit.md). The next-state [Boolean functions](../../../../../boolean-function.md) are

$$
\boxed{D_0=\neg q_0,\qquad D_1=q_1\oplus q_0,\qquad D_2=q_2\oplus(q_1\land q_0).}
$$

Implement these with one [NOT gate](../../../../../not-gate.md), two [exclusive or](../../../../../exclusive-or.md) gates, and one [AND gate](../../../../../and-gate.md). Connect each $D_i$ to its corresponding [D flip-flop](../../../../../d-flip-flop.md); its output $q_i$ is address line $i$. A reset input clears all three [flip-flops](../../../../../flip-flop.md) to zero, so the first selected sensor is sensor zero.

The state sequence is

$$
000\to001\to010\to011\to100\to101\to110\to111\to000.
$$

The low [bit](../../../../../bit.md) toggles at every [clock edge](../../../../../clock-edge.md), the middle [bit](../../../../../bit.md) toggles exactly when the old low [bit](../../../../../bit.md) is one, and the high [bit](../../../../../bit.md) toggles exactly when both old lower [bits](../../../../../bit.md) are one. These are precisely the [carry](../../../../../carry-arithmetic.md) conditions for incrementing a three-[bit](../../../../../bit.md) [binary representation](../../../../../binary-number.md). Every possible state belongs to the cycle, so there is no unused state requiring recovery. Choose a [clock period](../../../../../clock-period.md) allowing the [combinational logic](../../../../../combinational-logic.md) to settle before the next capture.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
