<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The original PDF has $\mathbb E|X_T|<\infty$ and $\mathbb E[|X_n|\mathbf1_{\{T>n\}}]\to0$. The TeX transcription drops the [expected value](../../../../../../expected-value.md) and absolute value in the first condition, and the absolute value in the second. The proof uses the PDF's conditions.

Because the [stopping time](../../../../../../stopping-time.md) $T$ is finite [almost surely](../../../../../../almost-sure-convergence.md), $X_{n\wedge T}\to X_T$ [almost surely](../../../../../../almost-sure-convergence.md). More strongly,

$$
\mathbb E|X_{n\wedge T}-X_T|
=\mathbb E\left[|X_n-X_T|\mathbf1_{\{T>n\}}\right]
\leq\mathbb E\left[|X_n|\mathbf1_{\{T>n\}}\right]
+\mathbb E\left[|X_T|\mathbf1_{\{T>n\}}\right]\longrightarrow0.
$$

The first term tends to zero by hypothesis; the second does so by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md). Thus there is [convergence in L1](../../../../../../convergence-in-l1.md).

Here is the needed [L1 convergence implies uniform integrability](../../../../../../l1-convergence-implies-uniform-integrability.md) argument. For any [integrable random variables](../../../../../../integrable-random-variable.md) $Z,Y$ and $K>0$, splitting according to $|Y|>K/2$ gives

$$
\mathbb E\left[|Z|\mathbf1_{\{|Z|>K\}}\right]
\leq2\mathbb E|Z-Y|+\mathbb E\left[|Y|\mathbf1_{\{|Y|>K/2\}}\right].
$$

Take $Z=X_{n\wedge T}$ and $Y=X_T$. For large $n$, the first term is uniformly small by [convergence in L1](../../../../../../convergence-in-l1.md), and the second is small for large $K$ by [integrability](../../../../../../integrable-random-variable.md). The finitely many remaining $n$ are handled individually by [integrability](../../../../../../integrable-random-variable.md). Hence **the stopped process is [uniformly integrable](../../../../../../uniform-integrability.md)**. This proves the [stopped-martingale uniform integrability criterion](../../../../../../stopped-martingale-uniform-integrability-criterion.md); the [martingale](../../../../../../martingale-split.md) assumption is not needed for this particular implication.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
