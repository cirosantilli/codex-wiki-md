<h1 id="22j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $\varphi(0)=1$ and $\varphi(h)+\varphi(-h)=2\mathbb E\cos(hX)$, the expression in the hypothesis equals $\mathbb E Z_n$, with $Z_n=2[1-\cos(h_nX)]/h_n^2\geq0$. For every finite real $X$, the Taylor expansion of cosine gives $Z_n\to X^2$. The [Fatou lemma](../../../../../../fatou-s-lemma.md) therefore gives

$$
\boxed{\mathbb E X^2\leq\liminf_n\frac{2\varphi(0)-\varphi(-h_n)-\varphi(h_n)}{h_n^2}<\infty.}
$$

No differentiability of the [characteristic function](../../../../../../characteristic-function.md) or prior integrability of $X^2$ was assumed; the nonnegative difference quotient establishes it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22J](../../22j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
