<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Convergence in the [Hilbert-Schmidt norm](../../../../../../../hilbert-schmidt-norm.md) implies

$$
\lVert L_i^p\rVert_{\mathrm{HS}}^2
\longrightarrow\lVert L_i\rVert_{\mathrm{HS}}^2.
$$

Products of two Hilbert-Schmidt operators are [trace-class operators](../../../../../../../trace-class-operator.md), and the [Schatten norm Hölder inequality](../../../../../../../schatten-norm-holder-inequality.md) gives

$$
\begin{aligned}
\lVert(L_2^p)^*L_1^p-L_2^*L_1\rVert_1
&\leq
\lVert L_2^p-L_2\rVert_{\mathrm{HS}}\lVert L_1^p\rVert_{\mathrm{HS}}\\
&\quad+\lVert L_2\rVert_{\mathrm{HS}}\lVert L_1^p-L_1\rVert_{\mathrm{HS}}
\longrightarrow0.
\end{aligned}
$$

By [trace duality](../../../../../../../trace-duality.md), every unitary $R$ satisfies

$$
\left|\operatorname{tr}\!\left(R^*\{(L_2^p)^*L_1^p-L_2^*L_1\}\right)\right|
\leq\lVert(L_2^p)^*L_1^p-L_2^*L_1\rVert_1.
$$

Taking the supremum over $R$ shows that the supremum terms in the two Procrustes formulas converge. Combining this with convergence of the squared norms proves

$$
\boxed{d_P(C_1^p,C_2^p)^2\longrightarrow d_P(C_1,C_2)^2.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 225](../../../../paper-225-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
