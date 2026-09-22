<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [D flip-flop](../../../../../d-flip-flop.md) stores one [bit](../../../../../bit.md). At its specified active [clock edge](../../../../../clock-edge.md), it samples $D$ and, after its [clock-to-Q delay](../../../../../clock-to-q-delay.md), makes $Q$ equal to that sampled value. Between active [clock edges](../../../../../clock-edge.md) it retains the stored value. The input must meet the [setup and hold time](../../../../../setup-and-hold-time.md) requirements around the sampling edge; a level-sensitive latch would have different behavior.

For a finite-state [sequential circuit](../../../../../sequential-logic.md), encode the present state in a bank of [D flip-flops](../../../../../d-flip-flop.md). Feed their outputs $q$ and the external inputs $u$ to [combinational logic](../../../../../combinational-logic.md) computing the next-state [function](../../../../../function-split.md) $F(q,u)$, and connect those outputs to the flip-flop $D$ inputs. A common [clock signal](../../../../../clock-signal.md) then performs the simultaneous update

$$
\boxed{q^+=F(q,u).}
$$

Output [combinational logic](../../../../../combinational-logic.md) computes $H(q)$ for a [Moore machine](../../../../../moore-machine.md) or $H(q,u)$ for a [Mealy machine](../../../../../mealy-machine.md). Since any finite next-state and output table is a [Boolean function](../../../../../boolean-function.md), it has a [Boolean circuit](../../../../../boolean-circuit.md) implementation. Initialization specifies the starting state, and unused state encodings require either a recovery rule or an initialization assumption. The [clock period](../../../../../clock-period.md) must accommodate propagation through the [D flip-flops](../../../../../d-flip-flop.md) and intervening [combinational logic](../../../../../combinational-logic.md) before the next sampling edge.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
