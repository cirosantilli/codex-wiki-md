<h1 id="1/a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Choose an [orthonormal basis](../../../../../../../orthonormal-basis.md) $(e_j)$ of the [separable Hilbert space](../../../../../../../separable-hilbert-space.md) and independent standard [normal random variables](../../../../../../../gaussian-random-variable.md) $(Z_j)$ on a common [probability space](../../../../../../../probability-space.md). In finite dimension the sums below are finite; in dimension zero take $X(0)=0$. In infinite dimension define

$$
S_N(h)=\sum_{j=1}^N\langle h,e_j\rangle Z_j.
$$

Independence, centring and unit variance give

$$
\mathbb E|S_N(h)-S_M(h)|^2=\sum_{j=M+1}^N\langle h,e_j\rangle^2\longrightarrow0.
$$

By the [Parseval identity for a Hilbertian basis](../../../../../../../parseval-identity-for-a-hilbertian-basis.md), the coefficient sequence is square-summable. Completeness of $L^2(\Omega)$ therefore supplies a limit, and we define

$$
\boxed{X(h)=\lim_{N\to\infty}S_N(h)\quad\text{in }L^2(\Omega).}
$$

Every partial-sum map is linear, and passage to the $L^2$ limit preserves this identity. Thus for each fixed $a,b,g,h$, $X(ag+bh)=aX(g)+bX(h)$ as an $L^2$ identity, hence an [almost sure equality](../../../../../../../almost-sure-equality.md). This constructs an [isonormal Gaussian process](../../../../../../../isonormal-gaussian-process.md).

The usual meaning is almost-sure linearity for each fixed choice of arguments. A version linear simultaneously for every argument can also be chosen: select a [Hamel basis](../../../../../../../basis.md) of $H$, choose a measurable representative of $X$ on each basis vector, and extend each sample algebraically by finite sums. For every fixed $h$, this extension equals the constructed $L^2$ variable almost surely, so all its required distributions are unchanged.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 25](../../../../paper-25-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
