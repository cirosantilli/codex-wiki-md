<h1 id="15d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $X|x\rangle=|x+1\rangle$ on the input register and let $N|y\rangle=|-y\rangle$ on the target register. Both are fixed [unitary operators](../../../../../../unitary-operator.md) independent of $f$. Conjugating the query by the input shift gives

$$
\boxed{U_{f_1}=(X^{-1}\otimes I)U_f(X\otimes I),}
$$

because the intermediate query is made at $x+1$. Conjugating by target negation gives

$$
\boxed{U_{f_2}=(I\otimes N)U_f(I\otimes N),}
$$

since $y\mapsto-y\mapsto-y+f(x)\mapsto y-f(x)$. Each construction uses $U_f$ exactly once.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
