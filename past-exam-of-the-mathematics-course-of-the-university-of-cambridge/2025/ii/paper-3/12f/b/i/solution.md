<h1 id="12f/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define the extended transition recursively by

$$
\widehat\Delta(q,\varepsilon)=\{q\},
\qquad
\widehat\Delta(q,wa)
=\bigcup_{p\in\widehat\Delta(q,w)}\Delta(p,a).
$$

The automaton accepts $w$ precisely when

$$
\boxed{w\in\mathcal L(N)
\quad\Longleftrightarrow\quad
\widehat\Delta(q_0,w)\cap F\ne\varnothing.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [12F](../../../12f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
