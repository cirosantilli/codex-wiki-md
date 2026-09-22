<h1 id="26k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $T(x)=x+\alpha\pmod1$ with irrational $\alpha$. This [irrational rotation of the circle](../../../../../../irrational-rotation.md) preserves [Lebesgue measure](../../../../../../lebesgue-measure.md) and is ergodic. Apply the [Birkhoff ergodic theorem](../../../../../../birkhoff-ergodic-theorem.md) to the [indicator function](../../../../../../indicator-function.md) $\mathbf1_A$. Its limit

$$
\mathbb E[\mathbf1_A\mid\mathcal I]
$$

is invariant, hence almost everywhere constant by [ergodicity](../../../../../../ergodicity.md). Its integral must equal that of $\mathbf1_A$, so the constant is $\mu(A)$. Therefore

$$
\boxed{
\frac{S_n(\mathbf1_A)(x)}n
=\frac1n\sum_{j=0}^{n-1}\mathbf1_A(T^jx)
\longrightarrow\mu(A)
}
$$

for [Lebesgue measure](../../../../../../lebesgue-measure.md)-almost every $x\in(0,1]$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26K](../../26k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
