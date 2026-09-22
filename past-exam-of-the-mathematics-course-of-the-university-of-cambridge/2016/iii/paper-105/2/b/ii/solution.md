<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose continuous representatives using [Morrey's inequality](../../../../../../../morrey-s-inequality.md). On the closed unit ball they are uniformly bounded by $C M$ and satisfy

$$
|u_n(x)-u_n(y)|\leq CM|x-y|^{1-d/p}.
$$

The [Arzelà-Ascoli theorem](../../../../../../../arzela-ascoli-theorem.md) therefore gives a uniformly convergent subsequence with a continuous limit. For $p=\infty$, use the uniform Lipschitz estimate instead; this part remains valid at that endpoint.

For [weak lower semicontinuity of the Hilbert norm](../../../../../../../weak-lower-semicontinuity-of-the-hilbert-norm.md), weak convergence gives $\langle u_n-\phi,\phi\rangle\to0$, and hence

$$
\|u_n\|^2=\|\phi\|^2+\|u_n-\phi\|^2+o(1).
$$

Taking the lower limit proves $\boxed{\|\phi\|\leq\liminf_n\|u_n\|}$.

For the nonlinear integral, use [local Sobolev compactness gives lower semicontinuity of a nonnegative integral](../../../../../../../local-sobolev-compactness-gives-lower-semicontinuity-of-a-nonnegative-integral.md). Select a subsequence attaining the lower limit of the integrals. The [Rellich-Kondrachov compactness theorem](../../../../../../../rellich-kondrachov-theorem.md) on successively larger balls gives a diagonal subsequence converging strongly in local [L2 space](../../../../../../../l2-space-is-a-hilbert-space.md) to $\phi$. After a further subsequence it converges almost everywhere. Since $1-\cos s\geq0$, the [Fatou lemma](../../../../../../../fatou-s-lemma.md) gives

$$
\boxed{\int_{\mathbb R^3}(1-\cos\phi)\,dx\leq\liminf_n\int_{\mathbb R^3}(1-\cos u_n)\,dx.}
$$

Each integral is finite because $0\leq1-\cos s\leq s^2/2$. The argument uses local compactness rather than convexity: $1-\cos s$ is not a convex function on the whole real line.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
