<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $N=p^n$, $\alpha=|A|/N$, and use normalized [Fourier analysis on a finite abelian group](../../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md). If $F=1_A*1_A$ denotes unnormalized convolution and $h=N^{-1}F$, then

$$
\widehat h(\gamma)=\widehat{1_A}(\gamma)^2,
\qquad
\sum_\gamma|\widehat h(\gamma)|
=\sum_\gamma|\widehat{1_A}(\gamma)|^2
=\alpha
$$

by the [Parseval identity](../../../../../../parseval-identity.md).

Sample $k=O(m\varepsilon^{-2})$ characters independently, choosing $\gamma$ with probability $|\widehat h(\gamma)|/\alpha$, and attach the phase of $\widehat h(\gamma)$ to the sampled character. The [Marcinkiewicz–Zygmund inequality](../../../../../../marcinkiewicz-zygmund-inequality.md), followed by averaging over $x$, shows that some sampled Fourier sum $g$ satisfies

$$
\|h-g\|_{L^{2m}(\mathbb E)}\leq\frac{\varepsilon\alpha}{2}.
$$

This is the sampling argument recorded in the [finite-field character approximation](../../../../../../finite-field-character-approximation.md) principle.

Let $V$ be the intersection of the kernels of the sampled characters. It is a [vector subspace](../../../../../../vector-subspace.md) of codimension at most $k$, and $\tau_tg=g$ for every $t\in V$. The [triangle inequality](../../../../../../triangle-inequality.md) therefore gives

$$
\|\tau_th-h\|_{L^{2m}(\mathbb E)}
\leq2\|h-g\|_{L^{2m}(\mathbb E)}
\leq\varepsilon\alpha.
$$

Returning from normalized convolution and normalized norm to $F$ and the counting norm multiplies the right side by $N^{1+1/(2m)}$. Hence

$$
\|\tau_tF-F\|_{2m}
\leq\varepsilon|A|N^{1/(2m)}
=\varepsilon|A|p^{n/(2m)}
$$

for every $t\in V$, proving the [finite-field convolution almost-periodicity theorem](../../../../../../finite-field-convolution-almost-periodicity-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
