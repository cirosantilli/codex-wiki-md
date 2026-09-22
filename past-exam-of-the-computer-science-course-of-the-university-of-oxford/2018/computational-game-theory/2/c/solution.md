<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each history of the first two votes, voter 3 selects its favourite achievable winner. Writing rows for voter 1's vote and columns for voter 2's vote, the resulting continuation winners are

$$
\begin{array}{c|ccc}
&A&B&C\\\hline
A&A&B&C\\
B&B&B&B\\
C&C&B&C
\end{array}.
$$

For example, after votes $B,C$, voter 3 can make either $B$ or $C$ win, and prefers $B$; a vote for $A$ would instead produce the tie-break winner $A$.

Voter 2 prefers $C$ to $B$ to $A$. Optimizing each row therefore gives continuation winners $C,B,C$ after voter 1's respective choices $A,B,C$. Voter 1 prefers $B$ to $C$ and therefore votes $B$, giving **winner $B$ in every [subgame perfect equilibrium](../../../../../subgame-perfect-equilibrium.md)**.

Some histories admit several equally good votes, but they produce the same winning candidate. Since each voter strictly ranks the three possible winners, [unique outcome under strict outcome preferences](../../../../../unique-outcome-under-strict-outcome-preferences.md) makes this winner independent of those action ties. This is [backward induction](../../../../../backward-induction.md) over outcomes, not a claim that the entire equilibrium strategy profile is unique.

## ↑ Ancestors (11)

1. [C](../c.md)
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
