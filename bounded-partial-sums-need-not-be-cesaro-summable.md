<h1 id="bounded-partial-sums-need-not-be-cesaro-summable">Bounded partial sums need not be Cesàro summable</h1>

↑ **Parent:** [Cesàro summation](cesaro-summation.md)

Construct [partial sums](partial-sum.md) $s_n$ from alternating blocks of zero and one, with lengths $1,3,9,27,\ldots$. Block $j$, beginning with $j=0$, has length $3^j$ and value zero when $j$ is [even](even-function.md), one when $j$ is [odd](odd-function.md). Define a [series](series-mathematics.md) by $a_0=s_0$ and $a_n=s_n-s_{n-1}$ for $n\geq1$; the [telescoping series](telescoping-series.md) identity recovers these chosen [partial sums](partial-sum.md). They remain in $[0,1]$.

At the end of odd block $2m+1$, the [Cesàro mean](cesaro-mean.md) is exactly $3/4$. At the end of even block $2m$, it is

$$
\frac{3(9^m-1)}{4(3\cdot9^m-1)}\longrightarrow\frac14.
$$

These two [subsequences](subsequence.md) have different [subsequential limits](subsequential-limit.md), so the [series](series-mathematics.md) has no first-order [Cesàro sum](cesaro-sum.md). A later block remains a substantial fraction of everything averaged so far. Boundedness alone therefore does not ensure a stable average.

<a id="image-periodic-partial-sums-have-a-stable-average-while-longer-alternating-blocks-prevent-a-cesaro-sum"></a>
![](cesaro-means-periodic-and-long-blocks.png)

**[Figure 6](#image-periodic-partial-sums-have-a-stable-average-while-longer-alternating-blocks-prevent-a-cesaro-sum). Periodic partial sums have a stable average, while longer alternating blocks prevent a Cesàro sum**. Original exact constructed [sequences](sequence.md). In the left panel, $s_n$ repeats $0,2,1$, giving [Cesàro means](cesaro-mean.md) tending to one. In the right panel, the [partial sums](partial-sum.md) alternate between blocks of zero and one whose lengths are powers of three. The horizontal axis uses the number $N+1$ of included [partial sums](partial-sum.md).

## ↑ Ancestors (9)

1. [Cesàro summation](cesaro-summation.md)
2. [Summation method](summation-method.md)
3. [Series (mathematics)](series-mathematics.md)
4. [Sequence and series](sequence-and-series-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cesàro mean](cesaro-mean.md)
- [Cesàro summation](cesaro-summation.md)
