<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $T=\inf\{t\geq0:X_t\notin(-a,b)\}$, and suppose the jumps of $X$ have absolute value at most $c$. A nonconstant centered finite-variance [Lévy process](../../../../../../levy-process.md) oscillates, so $T<\infty$ almost surely. Before $T$ the process lies in $(-a,b)$, and at $T$ its bounded overshoot gives $X_T\in[-a-c,b+c]$. Thus the variables $X_{T\wedge n}^2$ are uniformly bounded.

Apply the [optional sampling theorem for a supermartingale](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to the martingale from part (c):

$$
\mathbb E[X_{T\wedge n}^2]
=\sigma^2\mathbb E[T\wedge n].
$$

[Bounded convergence theorem](../../../../../../bounded-convergence-theorem.md) on the left and [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) on the right yield

$$
\boxed{\mathbb E[X_T^2]=\sigma^2\mathbb E[T].}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
