<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The pathwise identity $(S_t-S_{t-1})^2=S_t^2-S_{t-1}^2-2S_{t-1}(S_t-S_{t-1})$ telescopes to

$$
\sum_{t=1}^T(S_t-S_{t-1})^2
=S_T^2-S_0^2-2\sum_{t=1}^TS_{t-1}(S_t-S_{t-1}).
$$

This is the [discrete realized-variance replication identity](../../../../../../discrete-realized-variance-replication-identity.md). Replicate $S_T^2$ using part (b). Add a [self-financing portfolio](../../../../../../self-financing-portfolio.md) with initial wealth $-S_0^2$ and [stock](../../../../../../stock.md) holdings $-2S_{t-1}$ during $(t-1,t]$.

To give the cash positions explicitly, let

$$
G_{t-1}=-S_0^2-2\sum_{u=1}^{t-1}S_{u-1}(S_u-S_{u-1}).
$$

The added portfolio holds $G_{t-1}+2S_{t-1}^2$ units of the bond over that interval. Its starting value is $G_{t-1}$ and its change is exactly $-2S_{t-1}(S_t-S_{t-1})$. The combined holdings are therefore

$$
\boxed{\text{stock: }1-2S_{t-1},\quad
\text{bond: }G_{t-1}+2S_{t-1}^2,\quad
\text{calls: }2\text{ of each strike}.}
$$

The terminal value equals the squared-increment sum by the telescoping identity. Its initial cost is

$$
\boxed{S_0+2\sum_{K=1}^NC_0(K)-S_0^2
=2\sum_{K=1}^NC_0(K)+S_0(1-S_0).}
$$

The dynamic [stock](../../../../../../stock.md) hedge uses only prices known before each interval, while the calls remain static.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
