<h1 id="2/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The bounded [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives $\mathbb EX_{T\wedge n}=\mathbb EX_0$. Decompose the difference from the terminal value:

$$
X_{T\wedge n}-X_T=(X_n-X_T)\mathbf1_{\{T>n\}}.
$$

Consequently

$$
\mathbb E|X_{T\wedge n}-X_T|
\leq\mathbb E\bigl[|X_n|\mathbf1_{\{T>n\}}\bigr]
+\mathbb E\bigl[|X_T|\mathbf1_{\{T>n\}}\bigr]\longrightarrow0.
$$

The first term tends to zero by hypothesis. The second tends to zero by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), because $X_T$ is integrable and $T$ is finite with probability one. Thus the [stopped martingale](../../../../../../stopped-martingale.md) converges to $X_T$ with [convergence in L1](../../../../../../convergence-in-l1.md), which permits passage of expectations to the limit:

$$
\boxed{\mathbb EX_T=\mathbb EX_0.}
$$

The explicit tail condition supplies exactly the missing control for an unbounded [stopping time](../../../../../../stopping-time.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
