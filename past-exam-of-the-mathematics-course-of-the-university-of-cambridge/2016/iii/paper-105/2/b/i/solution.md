<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

On a bounded Lipschitz domain $\Omega\subset\mathbb R^d$, the [Rellich-Kondrachov compactness theorem](../../../../../../../rellich-kondrachov-theorem.md) states that $W^{1,p}(\Omega)\hookrightarrow L^q(\Omega)$ is compact for $1\leq p<\infty$ and

$$
\frac1q>\frac1p-\frac1d,
$$

with $1/q=0$ for $q=\infty$. Thus $q<p^*$ when $p<d$, every finite $q$ is allowed when $p=d$, and the embedding into continuous functions with their uniform norm is compact when $p>d$.

For the main proof, a [Sobolev extension operator](../../../../../../../sobolev-extension-operator.md) puts a bounded sequence into a common compactly supported region of $\mathbb R^d$. The [Sobolev fundamental theorem of calculus on lines](../../../../../../../sobolev-fundamental-theorem-of-calculus-on-lines.md) gives the uniform translation estimate $\|u(\cdot+h)-u\|_p\leq|h|\|\nabla u\|_p$. Convolution with a [mollifier](../../../../../../../mollifier.md) therefore approximates the sequence uniformly in [Lp space](../../../../../../../lp-space.md). At any fixed smoothing scale, its derivatives and supremum are uniformly bounded, so the [Arzelà-Ascoli theorem](../../../../../../../arzela-ascoli-theorem.md) gives a convergent subsequence. A diagonal choice and the uniform approximation give strong [Lp space](../../../../../../../lp-space.md) convergence. The finite measure of $\Omega$ handles $q<p$, while [Lp interpolation inequality](../../../../../../../lp-interpolation-inequality.md) with the bounded Sobolev embeddings upgrades this to the larger subcritical finite [Lp spaces](../../../../../../../lp-space.md); for $p>d$, [Morrey's inequality](../../../../../../../morrey-s-inequality.md) gives uniform equicontinuity directly and the [Arzelà-Ascoli theorem](../../../../../../../arzela-ascoli-theorem.md) gives uniform convergence. Boundedness of the domain is essential.

## ↑ Ancestors (12)

1. [I](../i.md)
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
