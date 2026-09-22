<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The mean increment is $\mathbb EX_1=-6/7+2/7=-4/7$, so $M_n=S_n+(4/7)n$ is a [martingale](../../../../../../martingale-split.md). Applying the bounded [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at $n\wedge T$ gives

$$
\mathbb E S_{n\wedge T}=-\frac47\mathbb E(n\wedge T).
$$

The terminal sums are bounded by the exit-state bounds from (b), while $n\wedge T$ increases to the integrable stopping time $T$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) on the left and the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) on the right therefore prove

$$
\boxed{\mathbb E S_T=-\frac47\mathbb ET.}
$$

This is also [Wald's equation](../../../../../../wald-s-equation.md) here. In fact, the stopped identity already implies $\mathbb E(n\wedge T)\leq7m/4$ from $S_{n\wedge T}\geq-m$, giving another direct finite-expectation justification.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
