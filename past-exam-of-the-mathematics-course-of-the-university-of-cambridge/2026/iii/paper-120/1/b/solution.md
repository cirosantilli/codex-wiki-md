<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Kripke completeness theorem for intuitionistic propositional logic](../../../../../../kripke-completeness-theorem-for-intuitionistic-propositional-logic.md) says

$$
\vdash_{IPC}\varphi
\quad\Longleftrightarrow\quad
w\Vdash\varphi
$$

for every world $w$ in every intuitionistic Kripke model.

Take a root $r$ with two incomparable successors $u,v$. Force $p$ but not $q$ at $u$, force $q$ but not $p$ at $v$, and force neither at $r$. Then $r\nVdash p\to q$ because of $u$, and $r\nVdash q\to p$ because of $v$. Hence

$$
r\nVdash(p\to q)\vee(q\to p),
$$

so completeness shows that this proposition is not intuitionistically valid.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
