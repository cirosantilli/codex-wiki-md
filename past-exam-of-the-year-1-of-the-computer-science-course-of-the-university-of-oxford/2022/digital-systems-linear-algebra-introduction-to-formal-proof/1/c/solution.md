<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply [comparator composition](../../../../../comparator-composition.md) recursively in a [balanced binary tree](../../../../../balanced-binary-tree.md), with one-[bit](../../../../../bit.md) [digital comparators](../../../../../digital-comparator.md) at its leaves. For a [power of two](../../../../../power-of-two.md) $n$, the [circuit size](../../../../../circuit-size.md) and [circuit depth](../../../../../depth-of-a-boolean-circuit.md) satisfy

$$
S(n)=2S(n/2)+O(1),\qquad D(n)=D(n/2)+O(1).
$$

There are $n$ leaves and $n-1$ internal nodes, so **the [circuit size](../../../../../circuit-size.md) is $O(n)$ and the combinational delay is $O(\log n)$**. Here each fixed-fan-in [logic gate](../../../../../logic-gate.md) has bounded delay. For arbitrary $n$, pad both inputs with leading zero [bits](../../../../../bit.md) to the next [power of two](../../../../../power-of-two.md), which is less than $2n$; this preserves their [unsigned interpretation](../../../../../unsigned-interpretation-of-a-bit-string.md) and both bounds.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
