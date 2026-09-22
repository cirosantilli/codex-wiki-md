<h1 id="17b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On the circular arc, $|z|=R$, the reverse [triangle inequality](../../../../../../triangle-inequality.md) gives $|1+z^n|\ge R^n-1$. The arc length is $2\pi R/n$, so the [ML inequality](../../../../../../estimation-lemma.md) gives

$$
\left|\int_{\gamma_R}f(z)\,dz\right|
\le\frac{2\pi R}{n}\frac{R^m}{R^n-1}
=O(R^{m+1-n})\longrightarrow0.
$$

The strict assumption $n>m+1$ is exactly what makes the exponent negative; it also ensures convergence of the positive-real-axis integral at infinity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17B](../../17b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
