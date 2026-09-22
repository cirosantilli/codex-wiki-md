<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [hidden subgroup problem](../../../../../../hidden-subgroup-problem.md) supplies an oracle $f:G\to X$ promised to satisfy

$$
f(g_1)=f(g_2)\quad\Longleftrightarrow\quad g_1H=g_2H
$$

for an unknown subgroup $H\leq G$; the task is to determine $H$.

For a function $f:\mathbb Z_K\to\mathbb Z$ with least period $r$ dividing $K$, use the additive group $G=\mathbb Z_K$ and hidden subgroup

$$
\boxed{H=\langle r\rangle
=\{0,r,2r,\ldots,K-r\}}.
$$

Its cosets are the residue classes modulo $r$. Periodicity makes $f$ constant on each coset, while injectivity within a period makes values on distinct cosets different. Determining $H$, or its least positive generator $r$, is exactly [quantum period finding](../../../../../../quantum-period-finding.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
