<h1 id="9/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Arrange each four-variable [Karnaugh map](../../../../../karnaugh-map.md) in [Gray code](../../../../../gray-code.md) order $LG=00,01,11,10$ down the rows and $ab=00,01,11,10$ across the columns. For $L^+$ the row strings are `0100`, `0100`, `----`, `1110`; for $G^+$ they are `0001`, `1011`, `----`, `0001`. The maps are drawn alongside the [state-transition diagram](../../../../../state-transition-diagram.md) above.

In the $L^+$ map, group the whole `ab=01` column to obtain $\neg a\land b$. Group rows `11,10` with columns `00,01` to obtain $L\land\neg a$. Group those same rows with columns `01,11` to obtain $L\land b$. The unused-state row permits these larger groups. Symmetrically, in the $G^+$ map group column `ab=10`, rows `01,11` with columns `11,10`, and those same rows with columns `10,00` (wrapping around the map). This gives

$$
\boxed{\begin{aligned}
L^+&=(\neg a\land b)\lor(L\land\neg a)\lor(L\land b),\\
G^+&=(a\land\neg b)\lor(G\land a)\lor(G\land\neg b).
\end{aligned}}
$$

These expressions drive the D inputs of the two [D flip-flops](../../../../../d-flip-flop.md). With $a=b$, both copy their stored [bit](../../../../../bit.md). With $ab=01$, they force `Lt`; with $ab=10$, they force `Gt`. The equations also specify a harmless extension at unused code `11`: equal inputs retain it and unequal inputs recover to a valid comparison state. Correct reset is still required. This extension was chosen using don't-cares; the circuit is not claimed to recover from every invalid state without reset.

## ↑ Ancestors (12)

1. [E](../e.md)
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
