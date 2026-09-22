<h1 id="9/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $(L^+,G^+)$ denote the state after the next active [clock edge](../../../../../clock-edge.md). In the [truth table](../../../../../truth-table.md), an entry is the two-bit next-state code, and `–` marks a don't-care value for the unused current state `11`:

| Current $LG$ | $ab=00$ | $ab=01$ | $ab=10$ | $ab=11$ |
| --- | --- | --- | --- | --- |
| $00$ (`Eq`) | $00$ | $10$ | $01$ | $00$ |
| $10$ (`Lt`) | $10$ | $10$ | $01$ | $10$ |
| $01$ (`Gt`) | $01$ | $10$ | $01$ | $01$ |
| $11$ (unused) | $--$ | $--$ | $--$ | $--$ |

For each input column, `01` forces $L^+G^+=10$, `10` forces $01$, and the two equal-input columns copy the current code. Thus this compact [truth table](../../../../../truth-table.md) specifies all twelve valid combinations of state and input, or twenty-four individual next-state [bits](../../../../../bit.md):

$$
\boxed{ab=01\Rightarrow(L^+,G^+)=(1,0),\quad
ab=10\Rightarrow(L^+,G^+)=(0,1).}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
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
