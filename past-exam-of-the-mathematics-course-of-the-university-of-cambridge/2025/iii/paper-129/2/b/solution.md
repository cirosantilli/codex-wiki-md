<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use normalized convolution and [Fourier coefficients](../../../../../../fourier-transform.md), and define the large spectrum

$$
\Gamma=\{\gamma\in\widehat G:|\widehat f(\gamma)|\geq\epsilon\delta\}.
$$

By the [Parseval identity](../../../../../../parseval-identity.md) and $0\leq f\leq1$,

$$
|\Gamma|\epsilon^2\delta^2
\leq\sum_\gamma|\widehat f(\gamma)|^2
=\mathbb E f^2
\leq\delta,
$$

so $|\Gamma|\leq\epsilon^{-2}\delta^{-1}$.

The [convolution theorem](../../../../../../convolution-theorem.md) gives

$$
(f*f*f)(x+y)-(f*f*f)(x)
=\sum_\gamma\widehat f(\gamma)^3\gamma(x)(\gamma(y)-1).
$$

If $y\in B(\Gamma,\epsilon)$, the part over $\Gamma$ is at most

$$
\epsilon\sum_{\gamma\in\Gamma}|\widehat f(\gamma)|^3
\leq\epsilon\delta\sum_\gamma|\widehat f(\gamma)|^2
\leq\epsilon\delta^2,
$$

because $|\widehat f(\gamma)|\leq\delta$. On the complementary spectrum, $|\widehat f(\gamma)|<\epsilon\delta$ and $|\gamma(y)-1|\leq2$, so the contribution is less than $2\epsilon\delta^2$. The required difference is therefore less than $3\epsilon\delta^2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
