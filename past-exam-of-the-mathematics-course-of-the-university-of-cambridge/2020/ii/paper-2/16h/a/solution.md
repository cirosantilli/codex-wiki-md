<h1 id="16h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define a [valuation](../../../../../../propositional-logic.md) $v$ on primitive propositions by

$$
v(p)=1\quad\Longleftrightarrow\quad p\in S.
$$

The assumptions say exactly that $S$ is a [maximal consistent set in propositional logic](../../../../../../maximal-consistent-set-in-propositional-logic.md). A structural induction on formulae proves

$$
v(t)=1\quad\Longleftrightarrow\quad t\in S.
$$

For example, consistency and the decision property give $\neg t\in S$ exactly when $t\notin S$, while deductive closure gives $s\land t\in S$ exactly when both $s,t\in S$; the other connectives follow similarly. Every member of $S$ is therefore true under $v$, so

$$
\boxed{v\text{ is a model of }S}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16H](../../16h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
