# Barrel shifter

↑ **Parent:** [Combinational logic](combinational-logic.md)

A [barrel shifter](barrel-shifter.md) moves a [machine word](machine-word.md) by a variable number of [bit](bit.md) positions through a bounded-depth [combinational logic](combinational-logic.md) circuit. For a $2^k$-bit [machine word](machine-word.md), cascade $k$ banks of [multiplexers](multiplexer.md) selecting optional shifts of $1,2,\ldots,2^{k-1}$. The binary shift-amount [bits](bit.md) select the stages; the chosen distances add. Logical shifts fill vacated positions with zero, whereas [bit rotations](bit-rotation.md) reconnect the discarded positions. A 32-bit logical [barrel shifter](barrel-shifter.md) can use five banks of 32 two-input [multiplexers](multiplexer.md).

## ↑ Ancestors (7)

1. [Combinational logic](combinational-logic.md)
2. [Boolean circuit](boolean-circuit.md)
3. [Circuit complexity](circuit-complexity.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Arithmetic logic unit](arithmetic-logic-unit.md)
- [Barrel shifter](barrel-shifter.md)
- [Bit rotation](bit-rotation.md)
- [Datapath](datapath.md)
- [Instruction pipelining](instruction-pipelining.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/3/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/3/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/3/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/3/e/solution.md)
- [Scaled index addressing](scaled-index-addressing.md)
