<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [STRIPS](../../../../../strips.md) action

$$
\begin{aligned}
\mathrm{Unload}(x,s):\quad
P&=\{\mathrm{isItem}(x),\mathrm{isBank}(s),
\mathrm{onBoat}(x),\mathrm{at}(\mathrm{BOAT},s)\},\\
A&=\{\mathrm{at}(x,s),\mathrm{Empty}\},\\
D&=\{\mathrm{onBoat}(x)\}.
\end{aligned}
$$

The onboard [precondition](../../../../../precondition.md) prevents inventing an item at a bank, and deleting $\mathrm{onBoat}(x)$ preserves the item's unique location. Restoring $\mathrm{Empty}$ preserves the one-item [planning state invariant](../../../../../planning-state-invariant.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
