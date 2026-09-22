<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [conjunction elimination](../../../../../../conjunction-elimination-rule.md) to extract the three inputs, then apply the [implication elimination rule](../../../../../../implication-elimination-rule.md) three times:

$$
\begin{array}{rll}
1&E\to(F\to(G\to H))&\text{premise}\\
2&\vert\ (E\land F)\land G&\text{assumption}\\
3&\vert\ E\land F&\land\text{-elim-L }2\\
4&\vert\ G&\land\text{-elim-R }2\\
5&\vert\ E&\land\text{-elim-L }3\\
6&\vert\ F&\land\text{-elim-R }3\\
7&\vert\ F\to(G\to H)&\to\text{-elim }1,5\\
8&\vert\ G\to H&\to\text{-elim }7,6\\
9&\vert\ H&\to\text{-elim }8,4\\
10&((E\land F)\land G)\to H&\to\text{-intro }2\text{--}9
\end{array}
$$

The [implication introduction rule](../../../../../../implication-introduction-rule.md) closes the only [subproof](../../../../../../subproof.md), giving

$$
\boxed{E\to F\to G\to H\ \vdash\ ((E\land F)\land G)\to H.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
