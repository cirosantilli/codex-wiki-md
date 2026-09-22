<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $F=(A\to C)\lor(B\to C)$ and $H=(A\lor B)\to C$, so the two displayed [propositional formulas](../../../../../propositional-formula.md) are $\varphi=F\to H$ and $\psi=H\to F$. Their complete [truth tables](../../../../../truth-table.md) are

$$
\begin{array}{ccc|cc|cc|cc}
A&B&C&A\to C&B\to C&F&H&\varphi&\psi\\\hline
0&0&0&1&1&1&1&1&1\\
0&0&1&1&1&1&1&1&1\\
0&1&0&1&0&1&0&0&1\\
0&1&1&1&1&1&1&1&1\\
1&0&0&0&1&1&0&0&1\\
1&0&1&1&1&1&1&1&1\\
1&1&0&0&0&0&0&1&1\\
1&1&1&1&1&1&1&1&1
\end{array}
$$

Therefore **$\psi$ is a [tautology](../../../../../tautology.md); $\varphi$ is not**. For example $(A,B,C)=(0,1,0)$ makes the antecedent $F$ true via $A\to C$, while $H$ is false because $B$ is true and $C$ is false. This explains why having just one of the two [logical implications](../../../../../logical-implication.md) is insufficient for the forward direction.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
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
