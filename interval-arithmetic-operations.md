# Interval arithmetic operations

↑ **Parent:** [Interval arithmetic](interval-arithmetic.md)

For [closed intervals](closed-real-interval.md) $X=[a,b]$ and $Y=[c,d]$, exact [addition](addition.md), [subtraction](subtraction.md) and [multiplication](multiplication.md) give

$$
\begin{aligned}
X+Y&=[a+c,b+d],\\
X-Y&=[a-d,b-c],\\
XY&=[\min\{ac,ad,bc,bd\},\max\{ac,ad,bc,bd\}].
\end{aligned}
$$

These [interval arithmetic operations](interval-arithmetic-operations.md) describe all results $u\mathbin{\circ}v$ for $(u,v)$ in the [Cartesian product](cartesian-product.md) $X\times Y$: the two inputs are allowed to vary independently. Independence here means freedom to choose either input anywhere in its [closed interval](closed-real-interval.md); it does not assert anything about [probability](probability.md). For example, $[1,2]+[3,5]=[4,7]$ and $[1,2]-[3,5]=[-4,-1]$.

All four endpoint [products](product-of-numbers.md) matter when signs change. For $X=[-2,3]$ and $Y=[-4,1]$, the endpoint [products](product-of-numbers.md) are $8,-2,-12,3$, so $XY=[-12,8]$. Taking just $ac$ and $bd$, even after sorting them, would give $[3,8]$ and lose valid negative [products](product-of-numbers.md).

For [division](division-mathematics.md), if $0\notin Y$, the [multiplicative inverse](multiplicative-inverse.md) gives $1/Y=[1/d,1/c]$ and $X/Y=X(1/Y)$. Thus $[1,2]/[3,4]=[1/4,2/3]$. This ordinary finite-[closed interval](closed-real-interval.md) rule requires a [denominator](denominator.md) that excludes zero. When the [denominator](denominator.md) contains zero, [division](division-mathematics.md) is undefined for some pairs and can become unbounded near zero; these formulas cannot supply a finite [interval enclosure](interval-enclosure.md) of all quotients. The operations above use exact endpoints; a computer implementation must also apply [outward rounding](outward-rounding.md).

**Table of contents**

- [Natural interval extension](natural-interval-extension.md)
  - [Interval dependency problem](interval-dependency-problem.md)
    - [Interval subdivision](interval-subdivision.md)
- [Interval square range](interval-square-range.md)

## ↑ Ancestors (6)

1. [Interval arithmetic](interval-arithmetic.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Interval arithmetic operations](interval-arithmetic-operations.md)
- [Natural interval extension](natural-interval-extension.md)
- [Outward rounding](outward-rounding.md)
