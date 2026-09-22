<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a single [read-only memory](../../../../../read-only-memory.md) implementing both the next-state and output equations, the address has four request bits plus three present-state bits. Each word contains three next-state bits and four grant bits. Hence

$$
\boxed{2^7\text{ words}\times7\text{ bits}=128\times7=896\text{ bits}.}
$$

Three [D flip-flops](../../../../../d-flip-flop.md) store the state outside this combinational ROM. This is the direct truth-table implementation for the encoding above. A smaller factored implementation exploits the independence of the next-state equations from $V$: a $64\times3$ next-state ROM and an $8\times4$ output ROM use $224$ stored bits in total, or the output decoder can be ordinary logic. These are different implementation organizations, not different state counts.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
