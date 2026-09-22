# Interval subdivision

↑ **Parent:** [Interval dependency problem](interval-dependency-problem.md)

[Interval subdivision](interval-subdivision.md) covers $X$ by smaller [closed intervals](closed-real-interval.md) $X_j$, computes a valid [interval enclosure](interval-enclosure.md) $F(X_j)$ on each, and takes their [union](set-union.md). Every allowed input belongs to a piece, so its output belongs to that [union](set-union.md). If one [closed interval](closed-real-interval.md) is wanted, take the smallest one containing the [union](set-union.md); gaps between separate output pieces can then be lost. Splitting narrows the freedom given to repeated inputs, while increasing the number of evaluations.

For $f(x)=x(1-x)$, split $[0,1]$ at $1/2$. The [natural interval extensions](natural-interval-extension.md) are

$$
\begin{aligned}
F([0,1/2])&=[0,1/2][1/2,1]=[0,1/2],\\
F([1/2,1])&=[1/2,1][0,1/2]=[0,1/2].
\end{aligned}
$$

Their [union](set-union.md) is $[0,1/2]$. Four equal pieces sharpen the upper bound again:

$$
\begin{array}{c|c|c}
X_j&[1,1]-X_j&F(X_j)\\\hline
[0,1/4]&[3/4,1]&[0,1/4]\\
[1/4,1/2]&[1/2,3/4]&[1/8,3/8]\\
[1/2,3/4]&[1/4,1/2]&[1/8,3/8]\\
[3/4,1]&[0,1/4]&[0,1/4]
\end{array}
$$

The [union](set-union.md) is now $[0,3/8]=[0,0.375]$, still wider than the actual [image of a function](image-of-a-function.md) $[0,1/4]$. These are exact [rational number](rational-number.md) bounds: the excess width comes from the [interval dependency problem](interval-dependency-problem.md), rather than [roundoff error](round-off-error.md).

## ↑ Ancestors (9)

1. [Interval dependency problem](interval-dependency-problem.md)
2. [Natural interval extension](natural-interval-extension.md)
3. [Interval arithmetic operations](interval-arithmetic-operations.md)
4. [Interval arithmetic](interval-arithmetic.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Interval arithmetic](interval-arithmetic.md)
- [Interval root exclusion](interval-root-exclusion.md)
- [Interval square range](interval-square-range.md)
- [Interval subdivision](interval-subdivision.md)
