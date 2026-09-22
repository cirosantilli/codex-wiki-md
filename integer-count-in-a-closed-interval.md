# Integer count in a closed interval

↑ **Parent:** [Floor and ceiling functions](floor-and-ceiling-functions.md)

For [real numbers](real-number.md) $a\leq b$, the [integers](integer.md) in the [closed interval](closed-real-interval.md) $[a,b]$ begin at $\lceil a\rceil$ and end at $\lfloor b\rfloor$, if there are any. Their number is therefore

$$
|[a,b]\cap\mathbb Z|=\max\!\left(0,\lfloor b\rfloor-\lceil a\rceil+1\right).
$$

The extra one includes both ends of the resulting [integer interval](integer-interval.md). The [maximum](maximum-of-a-subset-of-a-total-order.md) with zero handles an empty [intersection](set-intersection.md): $[0.2,0.8]$ contains no [integer](integer.md), even though it has positive length.

For $[-2.7,1.1]$, the [ceiling function](ceiling-function.md) selects $-2$ and the [floor function](floor-function.md) selects $1$, giving $1-(-2)+1=4$. The four points are $-2,-1,0,1$. For $[-2,2]$, the count is five, not four: the real length $2-(-2)$ and the number of [integer](integer.md) points are different quantities.

The endpoint convention matters. For the half-open [interval](interval-mathematics.md) $[a,b)$ with $a\leq b$, the last allowed [integer](integer.md) is $\lceil b\rceil-1$, so the count becomes $\max(0,\lceil b\rceil-\lceil a\rceil)$. This handles an [integer](integer.md) endpoint $b$ without including it accidentally. For example, $[-2,2)$ has four [integer](integer.md) points.

## ↑ Ancestors (7)

1. [Floor and ceiling functions](floor-and-ceiling-functions.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Floor and ceiling functions](floor-and-ceiling-functions.md)
