<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For every rational $0\leq a<b$, part a implies $U[a,b]<\infty$ almost surely. The intersection of these probability-one events over the countable collection of rational pairs still has probability one. On this event, if

$$
\liminf_nX_n<\limsup_nX_n,
$$

some rational interval $[a,b]$ lies strictly between them, forcing infinitely many upcrossings, a contradiction. Thus $X_n$ has an extended limit almost surely.

The limit cannot be $+\infty$ on a set of positive probability: [Fatou lemma](../../../../../../fatou-s-lemma.md) and the [supermartingale](../../../../../../supermartingale.md) property give

$$
\mathbb E[\liminf_nX_n]
\leq\liminf_n\mathbb E X_n
\leq\mathbb E X_0<\infty.
$$

Nonnegativity excludes $-\infty$. Therefore $X_n$ converges almost surely to a finite random variable, proving the [almost sure supermartingale convergence theorem](../../../../../../almost-sure-supermartingale-convergence-theorem.md) in this case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
