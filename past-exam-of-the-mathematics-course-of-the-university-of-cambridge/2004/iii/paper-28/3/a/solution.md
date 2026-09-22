<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the natural [filtration](../../../../../../filtration-probability-theory.md) $\mathcal G_n=\sigma(\xi_1,\ldots,\xi_n)$. Define the deterministic tail $r_n=\sum_{j=n}^\infty\delta_j$ and put $Z_n=\xi_n+r_n$. This is nonnegative and [integrable](../../../../../../integrability.md). Since $r_n=\delta_n+r_{n+1}$,

$$
\mathbb E[Z_{n+1}\mid\mathcal G_n]
\leq\xi_n+\delta_n+r_{n+1}=Z_n.
$$

Thus the [deterministic summable drift correction](../../../../../../deterministic-summable-drift-correction.md) produces a nonnegative [supermartingale](../../../../../../supermartingale.md). The [almost sure supermartingale convergence theorem](../../../../../../almost-sure-supermartingale-convergence-theorem.md) gives a finite limit $Z_\infty$ [almost surely](../../../../../../almost-sure-convergence.md). Its finiteness is also reflected in the bound $\mathbb EZ_n\leq\mathbb EZ_1$ and [Fatou's lemma](../../../../../../fatou-s-lemma.md), which gives $\mathbb EZ_\infty\leq\mathbb EZ_1<\infty$. The convergence theorem follows from the [upcrossing](../../../../../../upcrossing.md) argument: bounded expected negative parts of $-Z$ rule out infinitely many crossings of rational intervals, and the [expectation](../../../../../../expected-value.md) bound excludes an infinite limit.

Since $r_n\to0$, the required conclusion is $\boxed{\xi_n\longrightarrow Z_\infty\text{ almost surely, with }Z_\infty<\infty}$. The original sequence need not itself be a [supermartingale](../../../../../../supermartingale.md); subtracting the vanishing deterministic tail recovers it from one that is.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
