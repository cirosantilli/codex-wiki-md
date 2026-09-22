<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the [Curry-Howard correspondence](../../../../../../curry-howard-correspondence.md), the term takes a proof $p$ of $\phi\wedge\psi$, extracts proofs of $\phi$ and $\psi$, and applies $f:\phi\to(\psi\to\bot)$ to obtain a contradiction. It is therefore a proof of

$$
(\phi\wedge\psi)\to\bigl((\phi\to\neg\psi)\to\bot\bigr),
$$

equivalently $(\phi\wedge\psi)\to\neg(\phi\to\neg\psi)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
