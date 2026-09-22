<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $r$ be the number of true values among $a,b,c$. Count the ten [clause](../../../../../../clause-of-a-boolean-formula.md) occurrences for the two choices of $d$. With $d=0$, the three positive singletons contribute $r$, the three negated-pair [clauses](../../../../../../clause-of-a-boolean-formula.md) contribute $3-\binom r2$, and the last three [clauses](../../../../../../clause-of-a-boolean-formula.md) all hold. With $d=1$, the four singleton [clauses](../../../../../../clause-of-a-boolean-formula.md) contribute $r+1$, the negated pairs again contribute $3-\binom r2$, and the last three contribute $r$. Therefore

$$
\begin{array}{c|cc|c}
r&d=0&d=1&\text{maximum}\\\hline
0&6&4&6\\
1&7&6&7\\
2&7&7&7\\
3&6&7&7
\end{array}
$$

The original three-[literal](../../../../../../boolean-literal.md) [clause](../../../../../../clause-of-a-boolean-formula.md) is satisfied exactly when $r\ge1$, and then a value of $d$ satisfies exactly seven gadget [clauses](../../../../../../clause-of-a-boolean-formula.md). If $r=0$, no choice reaches seven. Thus **the required equivalence holds, and seven is also an upper bound for every assignment to the gadget.** This is the [seven-clause gadget for MAX-2SAT](../../../../../../seven-clause-gadget-for-max-2sat.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
