<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The generalized [quantile function](../../../../../../quantile-function.md) is

$$
\boxed{F^{-1}(u)=\inf\{x\in\mathbb R:F(x)\geq u\},\qquad0<u<1.}
$$

The tail limits of a [cumulative distribution function](../../../../../../cumulative-distribution-function.md) make the defining set nonempty and its infimum finite. Monotonicity and right continuity imply $F^{-1}(u)\leq x$ exactly when $u\leq F(x)$. To see the direction involving the infimum, let points in the defining set decrease towards it; right continuity gives $F(F^{-1}(u))\geq u$, so every larger $x$ also qualifies. Consequently, for a [uniform distribution](../../../../../../continuous-uniform-distribution.md) variable $U$,

$$
\mathbb P(F^{-1}(U)\leq x)=\mathbb P(U\leq F(x))=F(x).
$$

The probability-zero endpoints $U=0,1$ can be assigned arbitrary outputs. This proves [inverse transform sampling](../../../../../../inverse-transform-sampling.md) even for distributions with atoms or flat portions; continuity or strict monotonicity of $F$ is not required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
