<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Each waiting time has the [geometric distribution](../../../../../../geometric-distribution.md) on $1,2,\ldots$ with success probability $1/2$: a wait of length $n$ consists of $n-1$ failures followed by the prescribed success, so its probability is $2^{-n}$. Hence

$$
\boxed{G_{H_j}(s)=G_{T_j}(s)=\sum_{n\ge1}\left(\frac s2\right)^n=\frac{s}{2-s},\qquad
\mathbb E H_j=\mathbb E T_j=G'_{H_j}(1)=2.}
$$

Disjoint successive blocks of independent tosses give independent waiting times. More explicitly, any specified list of block lengths determines exactly one allowed sequence of heads and tails and has probability $2^{-\sum_j(h_j+t_j)}$, the product of the individual block probabilities.

There are $2r$ waiting times. Multiplication of their [probability generating functions](../../../../../../probability-generating-function.md) and addition of their [expectations](../../../../../../expected-value.md) give

$$
\boxed{G_{Y_r}(s)=\left(\frac{s}{2-s}\right)^{2r},\qquad \mathbb E Y_r=4r.}
$$

To recover its [probability mass function](../../../../../../probability-mass-function.md), expand by the [negative binomial series](../../../../../../negative-binomial-series.md):

$$
G_{Y_r}(s)=\frac{s^{2r}}{2^{2r}}(1-s/2)^{-2r}
=\frac{s^{2r}}{2^{2r}}\sum_{m\ge0}\binom{m+2r-1}{2r-1}(s/2)^m.
$$

The coefficient of $s^n$ is therefore

$$
\boxed{\mathbb P(Y_r=n)=2^{-n}\binom{n-1}{2r-1},\qquad n\ge2r,}
$$

and it is zero below $2r$. Equivalently there are $\binom{n-1}{2r-1}$ compositions of $n$ into $2r$ positive block lengths, each with probability $2^{-n}$. This is the [negative binomial distribution](../../../../../../negative-binomial-distribution.md) for a sum of geometric waiting times, even though the desired outcome alternates between blocks.

For $r=1$,

$$
\boxed{\mathbb P(Y_1\ge5)=1-\left(\frac14+\frac28+\frac3{16}\right)=\frac5{16}.}
$$

Since $\mathbb E Y_1=4$, [Markov's inequality](../../../../../../markov-inequality.md) gives $\mathbb P(Y_1\ge5)\le4/5$, and indeed $5/16<4/5$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Section II](../../section-ii.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
