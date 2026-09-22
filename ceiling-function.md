# Ceiling function

↑ **Parent:** [Floor and ceiling functions](floor-and-ceiling-functions.md)

The ceiling function gives the least [integer](integer.md) large enough to meet a real lower bound. For a [real number](real-number.md) $x$,

$$
\lceil x\rceil=m\quad\Longleftrightarrow\quad m-1<x\leq m,\qquad m\in\mathbb Z.
$$

Thus $\lceil2.7\rceil=3$, $\lceil-2.7\rceil=-2$, and $\lceil2\rceil=2$. The operation rounds upward in the [total order](total-order.md) on the [real numbers](real-number.md), which can move a negative input towards zero. Its difference from the input obeys $0\leq\lceil x\rceil-x<1$. Python's `math.ceil` implements this least-integer definition. [Python 3.14 math.ceil documentation: the least integer at least x](https://docs.python.org/3.14/library/math.html#math.ceil).

The [ceiling count for fixed-size batches](ceiling-count-for-fixed-size-batches.md) is a direct application. Suppose each box holds at most $k$ items, with positive [integer](integer.md) $k$, and there are $N\geq0$ items. The smallest number of boxes with enough capacity is $\lceil N/k\rceil$: a candidate count $b$ must satisfy $bk\geq N$. For $N=101$, $k=20$, **six boxes are needed**, leaving $120-101=19$ unused places. Exactly 100 items need only five boxes, and zero items need zero boxes. Adding one to the [floor function](floor-function.md) result unconditionally would therefore overcount at exact multiples of $k$.

<a id="image-the-ceiling-function-retains-the-endpoint-on-the-left-and-counts-enough-whole-containers"></a>
![](ceiling-function-thresholds-and-capacity.png)

**[Figure 2](#image-the-ceiling-function-retains-the-endpoint-on-the-left-and-counts-enough-whole-containers). The ceiling function retains the endpoint on the left and counts enough whole containers**. Left: open and filled endpoints distinguish the half-open [intervals](interval-mathematics.md) $(m-1,m]$ where $\lceil x\rceil=m$, including negative inputs. Right: the original capacity example uses 20 items per box; 101 items need six boxes, while an exact multiple of 20 needs no extra box. The right-hand inputs are integer item counts.

For nonnegative [integer](integer.md) $N$ and positive [integer](integer.md) $k$, [Euclidean division](euclidean-division.md) gives the exact identity

$$
\boxed{\left\lceil\frac Nk\right\rceil=\left\lfloor\frac{N+k-1}{k}\right\rfloor.}
$$

Write $N=qk+r$, $0\leq r<k$. The count is $q$ when the [remainder](remainder.md) is zero and $q+1$ otherwise, and the right-hand side encodes these two cases. This argument specifies the domain of the identity; arbitrary negative denominators require their own sign conventions.

The [ceiling function](ceiling-function.md) is a [nondecreasing function](nondecreasing-function.md), constant on each of the half-open [intervals](interval-mathematics.md) $(m-1,m]$, and has a [discontinuity of a function](discontinuity-of-a-function.md) at every [integer](integer.md). It is tied to the [floor function](floor-function.md) by $\lceil x\rceil=-\lfloor-x\rfloor$. Adding an [integer](integer.md) $j$ shifts its output by the same amount: $\lceil x+j\rceil=\lceil x\rceil+j$. At an [integer](integer.md) the floor and ceiling agree; at every other input they differ by one. These statements refer to exact [real numbers](real-number.md); an input already perturbed by [floating-point arithmetic](floating-point-arithmetic.md) can land on the other side of a threshold.

**Table of contents**

- [Ceiling count for fixed-size batches](ceiling-count-for-fixed-size-batches.md)

## ↑ Ancestors (7)

1. [Floor and ceiling functions](floor-and-ceiling-functions.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Bisection stopping criterion](bisection-stopping-criterion.md)
- [Cayley graphs of the integers](cayley-graphs-of-the-integers.md)
- [Ceiling count for fixed-size batches](ceiling-count-for-fixed-size-batches.md)
- [Ceiling function](ceiling-function.md)
- [Comparison sorting lower bound](comparison-sorting-lower-bound.md)
- [Floor and ceiling functions](floor-and-ceiling-functions.md)
- [Generalized pigeonhole principle](generalized-pigeonhole-principle.md)
- [Integer arithmetic](integer-arithmetic.md)
- [Integer count in a closed interval](integer-count-in-a-closed-interval.md)
- [Karatsuba operand splitting](karatsuba-operand-splitting.md)
- [Merge sort](merge-sort.md)
- [Mismatch penalty in lossless coding](mismatch-penalty-in-lossless-coding.md)
- [Natural density](natural-density.md)
- [Polled input-output](polled-input-output.md)
- [Remainder of a geometric series](remainder-of-a-geometric-series.md)
- [Truncation toward zero](truncation-toward-zero.md)
- [Uniform convergence](uniform-convergence.md)
