<h1 id="23i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\alpha$ be a [multi-index](../../../../../../multi-index-notation.md) with $|\alpha|\leq k$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\int_{\mathbb R^n}|\xi|^{|\alpha|}|\widehat u(\xi)|\,d\xi
\leq\lVert u\rVert_{H^s}
\left(\int_{\mathbb R^n}|\xi|^{2|\alpha|}(1+|\xi|^2)^{-s}\,d\xi\right)^{1/2}.
$$

The second integral is finite precisely under the sufficient inequality $s>|\alpha|+n/2$, which follows from $s>k+n/2$. Hence $(i\xi)^\alpha\widehat u$ is [Lebesgue integrable](../../../../../../lebesgue-integrable-function.md) for every $|\alpha|\leq k$.

The [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) therefore defines a function

$$
u^*(x)=(2\pi)^{-n}\int_{\mathbb R^n}e^{ix\cdot\xi}\widehat u(\xi)\,d\xi
$$

whose derivatives through order $k$ may be obtained by differentiating under the integral sign. Those derivatives are continuous, so $u^*\in C^k(\mathbb R^n)$. The inverse transform represents the same [tempered distribution](../../../../../../tempered-distribution.md) as $u$; consequently $u=u^*$ [almost everywhere](../../../../../../almost-everywhere.md). This is the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) $H^s(\mathbb R^n)\hookrightarrow C^k(\mathbb R^n)$ in this range.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [23I](../../23i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
