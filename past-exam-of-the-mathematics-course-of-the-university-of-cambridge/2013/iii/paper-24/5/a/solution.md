<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Skorokhod embedding of a centered random walk](../../../../../../skorokhod-embedding-of-a-centered-random-walk.md) states that a [random walk](../../../../../../random-walk.md) with independent identically distributed centered steps of finite [variance](../../../../../../variance-split.md) $\sigma^2$ can be realized on an appropriate probability space as

$$
S_n=B_{T_n},\qquad 0=T_0\leq T_1\leq T_2\leq\cdots,
$$

where $B$ is a standard [Brownian motion](../../../../../../brownian-motion-split.md) and the $T_n$ are finite [stopping times](../../../../../../stopping-time.md). More precisely, the stopped positions have the same joint law as the given [random walk](../../../../../../random-walk.md), and the pairs

$$
(T_n-T_{n-1},\,B_{T_n}-B_{T_{n-1}}),\qquad n\geq1,
$$

may be chosen independent and identically distributed. Their spatial component has the step law, and $\mathbb E(T_n-T_{n-1})=\sigma^2$. Repeating the one-step [Skorokhod embedding theorem](../../../../../../skorokhod-embedding-theorem.md) with the [Strong Markov property](../../../../../../strong-markov-property.md) gives this formulation. In the present normalization, the mean time increment is one, and the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $T_n/n\to1$ [almost surely](../../../../../../almost-sure-convergence.md).

The [Donsker invariance principle](../../../../../../donsker-s-theorem.md) states that the linearly interpolated diffusively rescaled [random walk](../../../../../../random-walk.md)

$$
W_n(t)=\frac{S_{\lfloor nt\rfloor}
+(nt-\lfloor nt\rfloor)X_{\lfloor nt\rfloor+1}}{\sqrt n},
\qquad 0\leq t\leq1,\qquad S_0=0,
$$

converges weakly as a random element of $C[0,1]$, equipped with the [uniform norm](../../../../../../supremum-norm.md), to standard [Brownian motion](../../../../../../brownian-motion-split.md) restricted to $[0,1]$. At $t=1$ the fractional term is zero. The only step assumptions needed here are zero mean, unit [variance](../../../../../../variance-split.md), and independent identical distributions; a higher moment or bounded support is not required. This is a [functional central limit theorem](../../../../../../donsker-s-theorem.md), concerning the entire interpolated path rather than only its endpoint.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
