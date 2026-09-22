<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At trial $k$, the [amplitude amplification theorem](../../../../../../amplitude-amplification.md) gives success probability

$$
p_k=\sin^2((2k+1)\theta).
$$

Because the state is prepared afresh, the probability that the first success occurs at $k$ is

$$
\boxed{
\Pr(k^*=k)=p_k\prod_{j=0}^{k-1}(1-p_j)
=\sin^2((2k+1)\theta)
\prod_{j=0}^{k-1}\cos^2((2j+1)\theta)}.
$$

If one application of $R$ uses a constant number of oracle calls, reaching and performing trial $k$ costs a total of order $1+2+\cdots+k=\Theta(k^2)$ calls. Equivalently,

$$
\mathbb E C
=\Theta\left(
\sum_{k\geq1}k
\prod_{j=0}^{k-1}\cos^2((2j+1)\theta)
\right).
$$

For $k\theta\ll1$, use $\log\cos^2x=-x^2+O(x^4)$ and

$$
\sum_{j=0}^{k-1}(2j+1)^2=\frac{k(4k^2-1)}3
$$

to obtain

$$
\Pr(k^*\geq k)
=\exp\left[-\frac43\theta^2k^3+o(\theta^2k^3)\right].
$$

The first successful index is therefore typically $k^*=\Theta(\theta^{-2/3})$, and

$$
\boxed{\mathbb E C=\Theta(\theta^{-4/3})
=\Theta((n^*)^{4/3})},
$$

where $n^*=\Theta(1/\theta)$ is the first near-optimal Grover iteration count.

The last requested assertion in the official paper is false as printed. In fact, for small $\theta$, at least a constant fraction of the indices $j<n^*$ have $(2j+1)\theta\geq\pi/4$, and hence failure probability at most $1/2$. Consequently

$$
\boxed{\Pr(k^*\geq n^*)
=\prod_{j=0}^{n^*-1}\cos^2((2j+1)\theta)
\leq 2^{-c n^*}\longrightarrow0}
$$

for some constant $c>0$, rather than being bounded below by a positive constant. The reversed event $\Pr(k^*<n^*)$ does have a positive lower bound and in fact tends to one.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
