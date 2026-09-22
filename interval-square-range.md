# Interval square range

↑ **Parent:** [Interval arithmetic operations](interval-arithmetic-operations.md)

The [interval square range](interval-square-range.md) treats squaring as one [function](function-split.md) of one input. For $X=[a,b]$ it is exactly

$$
\operatorname{sqr}([a,b])=
\begin{cases}
[0,\max\{a^2,b^2\}],&a\leq0\leq b,\\
[\min\{a^2,b^2\},\max\{a^2,b^2\}],&\text{otherwise}.
\end{cases}
$$

It retains the relationship that ordinary interval [multiplication](multiplication.md) loses: for $Z=[-1/2,1/2]$, the [interval square range](interval-square-range.md) is $[0,1/4]$, whereas the independent-input [product](product-of-numbers.md) $ZZ$ is $[-1/4,1/4]$.

Consequently, [completing the square](completing-the-square.md) for $x(1-x)$ and using the [interval square range](interval-square-range.md) gives

$$
Z=X-[1/2,1/2]=[-1/2,1/2],\qquad [1/4,1/4]-\operatorname{sqr}(Z)=[0,1/4].
$$

This is the exact [image of a function](image-of-a-function.md) on $X=[0,1]$. Merely rewriting the expression and evaluating $[1/4,1/4]-ZZ$ gives $[0,1/2]$, so it does not achieve the same sharpening. A mathematical $Z^2$ must be interpreted explicitly here: a [square range operation](interval-square-range.md) and an independent-input interval [product](product-of-numbers.md) have different meanings. Choosing an operation that preserves known structure can save many steps of [interval subdivision](interval-subdivision.md).

## ↑ Ancestors (7)

1. [Interval arithmetic operations](interval-arithmetic-operations.md)
2. [Interval arithmetic](interval-arithmetic.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Interval arithmetic](interval-arithmetic.md)
- [Interval dependency problem](interval-dependency-problem.md)
- [Interval root exclusion](interval-root-exclusion.md)
- [Interval square range](interval-square-range.md)
