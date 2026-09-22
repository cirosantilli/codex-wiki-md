<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define $Z_n=\sup_{m\geq n}|X_m-X|$. Then $0\leq Z_n\leq2$ and $Z_n\downarrow0$ almost surely. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives $\mathbb E Z_n\to0$.

Set $W_n=\mathbb E[Z_n\mid\mathcal F_n]$. Since $Z_{n+1}\leq Z_n$, the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives

$$
\mathbb E[W_{n+1}\mid\mathcal F_n]
=\mathbb E[Z_{n+1}\mid\mathcal F_n]
\leq W_n,
$$

so $(W_n)$ is a nonnegative [supermartingale](../../../../../../supermartingale.md). The [almost sure supermartingale convergence theorem](../../../../../../almost-sure-supermartingale-convergence-theorem.md) gives $W_n\to W_\infty$ almost surely, and [Fatou lemma](../../../../../../fatou-s-lemma.md) yields $\mathbb EW_\infty\leq\liminf_n\mathbb EW_n=0$. Hence $W_n\to0$ almost surely; because $\mathbb EW_n=\mathbb EZ_n\to0$, convergence also holds in $L^1$.

Finally,

$$
\left|\mathbb E[X_n\mid\mathcal F_n]-\mathbb E[X\mid\mathcal F_\infty]\right|
\leq W_n
+\left|\mathbb E[X\mid\mathcal F_n]-\mathbb E[X\mid\mathcal F_\infty]\right|.
$$

The second term tends to zero almost surely and in $L^1$ by part b. The first does so by the preceding argument, proving the [moving-variable conditional-expectation convergence](../../../../../../moving-variable-conditional-expectation-convergence.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
