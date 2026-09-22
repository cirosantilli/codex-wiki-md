<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With zero framings, the [surgery linking matrix](../../../../../../surgery-linking-matrix.md) is

$$
Q_2=J_n-I_n.
$$

Its eigenvalues are $n-1$ on the span of $(1,\ldots,1)$ and $-1$ on the complementary subspace, so $\det Q_2=(-1)^{n-1}(n-1)$. For $n>1$, its [Smith normal form](../../../../../../smith-normal-form.md) is $\operatorname{diag}(1,\ldots,1,n-1)$, and therefore

$$
H_i(S^3_{\widehat L_2};\mathbb Z)\cong
\begin{cases}
\mathbb Z,&i=0,3,\\
\mathbb Z/(n-1),&i=1,\\
0,&\text{otherwise}.
\end{cases}
$$

Handle slides reduce this surgery diagram to the standard surgery diagram of the [lens space](../../../../../../lens-space.md) $L(n-1,1)$; equivalently, the generator of the cokernel has linking pairing $1/(n-1)$. Thus

$$
\boxed{S^3_{\widehat L_2}\cong L(n-1,1)}
$$

up to the orientation convention for surgery. When $n=1$, the matrix is $(0)$ and the exceptional answer is $S^1\times S^2$, with $H_1\cong H_2\cong\mathbb Z$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
