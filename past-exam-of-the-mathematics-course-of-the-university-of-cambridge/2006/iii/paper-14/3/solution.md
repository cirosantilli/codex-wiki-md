<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Colour every vertex independently red or blue, each with [probability](../../../../../probability.md) $1/2$. A fixed $r$-element [hypergraph edge](../../../../../edge-of-a-hypergraph.md) is [monochromatic](../../../../../monochromatic-set.md) with [probability](../../../../../probability.md) $2^{1-r}$. If there are $m<2^{r-1}$ [hypergraph edges](../../../../../edge-of-a-hypergraph.md), the expected number of [monochromatic](../../../../../monochromatic-set.md) [hypergraph edges](../../../../../edge-of-a-hypergraph.md) is $m2^{1-r}<1$. Equivalently, the [union bound](../../../../../boole-s-inequality.md) says that the [probability](../../../../../probability.md) of even one [monochromatic](../../../../../monochromatic-set.md) [hypergraph edge](../../../../../edge-of-a-hypergraph.md) is less than one. **A proper two-colouring therefore exists.**

For the converse, suppose $r\geq2$, put $N=2r^2$, and sample $m$ [independent](../../../../../independent-random-variables.md) uniformly random $r$-subsets of an $N$-vertex set. Initially this is a [multihypergraph](../../../../../multihypergraph.md). For a fixed two-colouring with $a$ red vertices, a sampled [hypergraph edge](../../../../../edge-of-a-hypergraph.md) is [monochromatic](../../../../../monochromatic-set.md) with [probability](../../../../../probability.md)

$$
q(a)=\frac{\binom ar+\binom{N-a}r}{\binom Nr}.
$$

The numerator is minimized by $a=N/2=r^2$. To see this discretely, use $\binom{a+1}r-\binom ar=\binom a{r-1}$: the successive difference of the numerator is $\binom a{r-1}-\binom{N-a-1}{r-1}$, negative up to the middle and positive afterwards. [Binomial coefficients](../../../../../binomial-coefficient.md) with an upper index below $r$ are understood as zero.

For this balanced colouring,

$$
q(a)\geq2\frac{\binom{r^2}r}{\binom{2r^2}r}
=2^{1-r}\prod_{j=0}^{r-1}\frac{1-j/r^2}{1-j/(2r^2)}
\geq2^{1-r}\prod_{j=0}^{r-1}(1-j/r^2).
$$

The elementary inequality $\prod_j(1-u_j)\geq1-\sum_j u_j$, valid for $0\leq u_j\leq1$, gives

$$
q(a)\geq2^{1-r}\left(1-\frac{r(r-1)}{2r^2}\right)>2^{-r}.
$$

Thus any fixed colouring is proper for all the sampled [hypergraph edges](../../../../../edge-of-a-hypergraph.md) with [probability](../../../../../probability.md) at most $e^{-m2^{-r}}$. There are $2^N$ colourings, so choose

$$
m=\left\lceil(N\log2+1)2^r\right\rceil.
$$

A [union bound](../../../../../boole-s-inequality.md) makes the [probability](../../../../../probability.md) that any proper colouring exists at most $2^Ne^{-m2^{-r}}\leq e^{-1}<1$. Some sampled [multihypergraph](../../../../../multihypergraph.md) is consequently not two-colourable. Remove repeated copies of its [hypergraph edges](../../../../../edge-of-a-hypergraph.md): this changes neither which colourings are proper nor non-two-colourability, and leaves at most $m$ distinct [hypergraph edges](../../../../../edge-of-a-hypergraph.md). We have proved

$$
\boxed{\text{There is an }r\text{-uniform hypergraph without Property B with }O(r^22^r)\text{ edges}.}
$$

For $r=1$, one singleton [hypergraph edge](../../../../../edge-of-a-hypergraph.md) is already not two-colourable, so that endpoint causes no exception.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
