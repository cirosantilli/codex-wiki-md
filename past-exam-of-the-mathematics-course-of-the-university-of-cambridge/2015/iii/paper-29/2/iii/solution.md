<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Recall the [stopping-time sigma-algebra](../../../../../../stopping-time-sigma-algebra.md):

$$
\mathcal F_S=\{A\in\mathcal F:A\cap\{S\leq t\}\in\mathcal F_t\text{ for every }t\geq0\}.
$$

For the proposed random time,

$$
\{U\leq t\}=\bigl(A\cap\{S\leq t\}\bigr)\cup\bigl(A^c\cap\{T\leq t\}\bigr).
$$

The first set belongs to $\mathcal F_t$. Since $S\leq T$, the second can be written

$$
A^c\cap\{T\leq t\}=\{T\leq t\}\setminus\bigl(A\cap\{S\leq t\}\bigr),
$$

which also belongs to $\mathcal F_t$. Therefore **$U$ is a [stopping time](../../../../../../stopping-time.md)**, as in [pasting ordered stopping times](../../../../../../pasting-ordered-stopping-times.md). Moreover $S\leq U\leq T$, so $U$ is a [bounded stopping time](../../../../../../bounded-stopping-time.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
