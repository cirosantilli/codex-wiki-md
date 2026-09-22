# First return to equal counts in sampling without replacement

↑ **Parent:** [Sampling without replacement](sampling-without-replacement.md)

Draw balls sequentially without replacement from $g$ green and $r$ red balls. Let $T$ be the first positive draw count at which the numbers of drawn green and red balls agree. For $1\leq m\leq\min(g,r)$,

$$
\mathbb P(T=2m)=2C_{m-1}\frac{(g)_m(r)_m}{(g+r)_{2m}},
\qquad C_k=\frac1{k+1}\binom{2k}{k},
$$

where $(q)_j=q(q-1)\cdots(q-j+1)$ denotes the [falling factorial](falling-factorial.md) and $C_k$ is a [Catalan number](catalan-number.md). Odd [first return times](first-return-time.md) are impossible because equality requires an even total number of draws.

To count the successful colour orders, encode green by a step $+1$ and red by a step $-1$. If the first step is positive, a [first return time](first-return-time.md) $2m$ means that the [partial sums](partial-sum.md) remain strictly positive until the last step. Delete the first positive step and the last negative step, and shift the remaining heights down by one. The result is a [Dyck path](dyck-path.md) of length $2m-2$, of which there are $C_{m-1}$. Interchanging the colours doubles this count. Every such colour order has the same [probability](probability.md) under [sampling without replacement](sampling-without-replacement.md), namely $(g)_m(r)_m/(g+r)_{2m}$, proving the formula. In particular, the numbers of successful colour orders at lengths two, four and six are two, two and four; balanced orders with an earlier return must not be counted.

## ↑ Ancestors (7)

1. [Sampling without replacement](sampling-without-replacement.md)
2. [Probability sampling](probability-sampling.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
