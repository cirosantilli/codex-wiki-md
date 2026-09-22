<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Yes: let the order be voter 2, then voter 3, then voter 1.** When voter 1 moves last, it makes $A$ win whenever that is possible; otherwise it prefers $B$ to $C$. For the first two votes in this new order, its optimal continuation winners are

$$
\begin{array}{c|ccc}
&A&B&C\\\hline
A&A&A&A\\
B&A&B&A\\
C&A&A&C
\end{array}.
$$

Rows now record voter 2's initial choice and columns voter 3's choice. In a three-way split, the specified tie-break produces $A$, which explains, for example, the off-diagonal $B,C$ entry.

Voter 3 optimizes its ranking $B\succ C\succ A$ in each row, giving the continuation winners $A,B,C$. Voter 2 then chooses $C$, its favourite of the three. The winner is therefore **$C$ in every [subgame perfect equilibrium](../../../../../subgame-perfect-equilibrium.md)**, again by [unique outcome under strict outcome preferences](../../../../../unique-outcome-under-strict-outcome-preferences.md). In particular, if voter 2 starts with $C$, voter 3 must also vote $C$: either other vote lets the last voter force $A$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2018](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
