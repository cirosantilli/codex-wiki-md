<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\tau_n$ localize the nonnegative local martingale $M$. For $s\leq t$,

$$
\mathbb E(M_{t\wedge\tau_n}\mid\mathcal F_s)=M_{s\wedge\tau_n}.
$$

[Conditional Fatou lemma](../../../../../../conditional-fatou-lemma.md) and nonnegativity give

$$
\mathbb E(M_t\mid\mathcal F_s)
\leq\liminf_nM_{s\wedge\tau_n}=M_s.
$$

**Thus $M$ is a [supermartingale](../../../../../../supermartingale.md), recovering the general fact about a [nonnegative local martingale](../../../../../../nonnegative-local-martingale.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
