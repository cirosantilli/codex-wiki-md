# Floor and ceiling functions

↑ **Parent:** [Calculus](calculus-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Floor_and_ceiling_functions)

The [floor function](floor-function.md) and [ceiling function](ceiling-function.md) turn a [real number](real-number.md) into directed [integer](integer.md) bounds. They answer two different questions: which [integer](integer.md) is the largest one that does not exceed $x$, and which is the smallest one that is not less than $x$?

$$
\lfloor x\rfloor\leq x<\lfloor x\rfloor+1,\qquad
\lceil x\rceil-1<x\leq\lceil x\rceil.
$$

Both outputs are [integers](integer.md). These are exact mathematical operations; they need not choose the closest [integer](integer.md), and they do not refer to [roundoff error](round-off-error.md) in [floating-point arithmetic](floating-point-arithmetic.md).

For example,

$$
\begin{array}{c|r|r|r}
x&\lfloor x\rfloor&\lceil x\rceil&\{x\}\\\hline
2.7&2&3&0.7\\
2&2&2&0\\
-2.7&-3&-2&0.3\\
-2&-2&-2&0
\end{array}
$$

The [fractional part](fractional-part.md) is $\{x\}=x-\lfloor x\rfloor$. The negative example matters: discarding the digits after the decimal point would give $-2$, which is [truncation toward zero](truncation-toward-zero.md), rather than the [floor function](floor-function.md)'s value $-3$. At an [integer](integer.md), the [floor function](floor-function.md) and [ceiling function](ceiling-function.md) agree and the [fractional part](fractional-part.md) vanishes.

<a id="image-floor-and-ceiling-give-enclosing-integers-fractional-part-repeats-on-each-unit-interval"></a>
![](floor-ceiling-and-fractional-part.png)

**[Figure 1](#image-floor-and-ceiling-give-enclosing-integers-fractional-part-repeats-on-each-unit-interval). Floor and ceiling give enclosing integers; fractional part repeats on each unit interval**.

The usefulness is a bridge from continuous quantities to discrete decisions. An [integer count in a closed interval](integer-count-in-a-closed-interval.md) uses both bounds. A [ceiling count for fixed-size batches](ceiling-count-for-fixed-size-batches.md) counts how many containers or pages are needed; a [floor function](floor-function.md) counts how many complete groups fit. In [Euclidean division](euclidean-division.md), the same bounds specify the quotient, while the [fractional part](fractional-part.md) records the scaled [remainder](remainder.md). A small amount of notation removes many cases that would otherwise have to be stated separately.

The reflection identity

$$
\lceil x\rceil=-\lfloor-x\rfloor
$$

follows by reflecting the ordered [integers](integer.md) across zero: the largest one below $-x$ becomes the smallest one above $x$. For every [integer](integer.md) $m$, translation gives $\lfloor x+m\rfloor=\lfloor x\rfloor+m$ and $\lceil x+m\rceil=\lceil x\rceil+m$. These formulas turn upper bounds into lower bounds and move examples between neighboring [intervals](interval-mathematics.md).

For a historical example of the notation in use, Kenneth E. Iverson's 1962 conference paper _A Programming Language_ lists the [floor function](floor-function.md), [ceiling function](ceiling-function.md) and residue operation alongside the ordinary [arithmetic operations](arithmetic-operation.md). It states the two defining inequalities above, then extends operations component by component to [vectors](vector.md) and [matrices](matrix.md). This shows their role as tools for describing [algorithms](algorithm.md), rather than merely conventions for writing decimal numbers. [Iverson, A Programming Language, AFIPS Spring Joint Computer Conference, May 1962, Basic Operations; transcription with typography changes documented at the end](https://www.jsoftware.com/papers/AFIPS196205a.htm)

**Table of contents**

- [Integer count in a closed interval](integer-count-in-a-closed-interval.md)
- [Floor function](floor-function.md)
  - [Fractional part](fractional-part.md)
- [Ceiling function](ceiling-function.md)
  - [Ceiling count for fixed-size batches](ceiling-count-for-fixed-size-batches.md)
- [Truncation toward zero](truncation-toward-zero.md)

## ↑ Ancestors (6)

1. [Calculus](calculus-split.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
