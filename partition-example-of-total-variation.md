# Partition example of total variation

↑ **Parent:** [Total variation of a function](total-variation-of-a-function.md)

Define a [piecewise linear function](piecewise-linear-function.md) by joining the five points $(0,0),(1,2),(2,-1),(3,3),(4,1)$. Its net change is $1$, but the increments at these knots are $2,-3,4,-2$. Their [absolute values](absolute-value.md) give

$$
\boxed{V_0^4(f)=2+3+4+2=11.}
$$

This is its exact total variation, not merely one lower bound. Given any [partition of an interval](partition-of-an-interval.md), insert all five knots. The [triangle inequality](triangle-inequality.md) ensures that this [partition refinement](partition-refinement.md) cannot decrease the sum. On each resulting [monotone function](monotonic-function.md) segment, the absolute increments telescope, so every refined sum is $11$. The knot [partition of an interval](partition-of-an-interval.md) itself attains $11$.

<a id="image-a-piecewise-linear-function-has-net-change-1-and-total-variation-11-refinements-reveal-hidden-movement-while-accumulated-rises-and-falls-give-its-jordan-decomposition"></a>
![](total-variation-partition-refinement-and-jordan.png)

**[Figure 22](#image-a-piecewise-linear-function-has-net-change-1-and-total-variation-11-refinements-reveal-hidden-movement-while-accumulated-rises-and-falls-give-its-jordan-decomposition). A piecewise linear function has net change 1 and total variation 11; refinements reveal hidden movement, while accumulated rises and falls give its Jordan decomposition**.

Sampling only at $0,4$ gives $1$. Sampling at $0,1,3,4$ gives $2+1+2=5$. Inserting the remaining knot at $2$ reveals the descent and rise that were hidden inside $[1,3]$, giving $11$. These are nested [partitions of an interval](partition-of-an-interval.md): their sums increase because each is a [partition refinement](partition-refinement.md) of the preceding one. Arbitrarily chosen unrelated [partitions of an interval](partition-of-an-interval.md) need not produce an increasing sequence of sums.

## ↑ Ancestors (7)

1. [Total variation of a function](total-variation-of-a-function.md)
2. [Riemann integration](riemann-integration.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Integration error controlled by total variation](integration-error-controlled-by-total-variation.md)
- [Jordan decomposition of a function of bounded variation](jordan-decomposition-of-a-function-of-bounded-variation.md)
- [Uniformly small functions with nonvanishing total variation](uniformly-small-functions-with-nonvanishing-total-variation.md)
