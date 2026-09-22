<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Store two [bits](../../../../../bit.md): the output $z$, initially zero, and an `armed` [bit](../../../../../bit.md) $e$, initially one. Define the [synchronous sequential circuit](../../../../../synchronous-sequential-circuit.md) by

$$
\boxed{z'=z\mathbin{\oplus}(e\land c),\qquad e'=d\lor(e\land\neg c).}
$$

Here $\oplus$ is [exclusive or](../../../../../exclusive-or.md), and the input restriction $c\land d=0$ excludes conflicting commands. The output is the current stored $z$.

When armed, a sampled $c=1$ toggles $z$ and clears $e$. Further $c$ samples leave the output unchanged. A sampled $d=1$ sets $e=1$ without changing $z$, allowing a later $c$ to toggle it again. The same [clock edge](../../../../../clock-edge.md) cannot both rearm and trigger because $c,d$ are never simultaneously high. Thus the first $c$ toggles from zero to one, and subsequent toggles each require a new $d$ followed by a later $c$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
