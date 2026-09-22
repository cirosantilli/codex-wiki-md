<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use two stored [bits](../../../../../bit.md) $(L,G)$ with symmetric meanings:

$$
\boxed{\mathrm{Lt}=10,\qquad\mathrm{Eq}=00,\qquad\mathrm{Gt}=01.}
$$

Swapping the two numbers interchanges $L$ and $G$ and fixes equality. Decode the outputs by

$$
\boxed{x=L,\qquad y=\neg L\land\neg G,\qquad z=G.}
$$

Thus only the equality output needs extra [logic gates](../../../../../logic-gate.md), namely two inversions and an AND gate, or a NOR gate. Code `11` is unused. Initialize both [D flip-flops](../../../../../d-flip-flop.md) to zero before a new pair of numbers so the starting state is `Eq`. In normal operation only the three valid codes are reachable.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
