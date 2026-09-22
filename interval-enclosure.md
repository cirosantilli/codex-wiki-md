# Interval enclosure

↑ **Parent:** [Interval arithmetic](interval-arithmetic.md)

An [interval enclosure](interval-enclosure.md) $F(X)=[L,U]$ for a real-valued [function](function-split.md) $f$ on a [closed interval](closed-real-interval.md) $X$ satisfies

$$
L\leq f(x)\leq U\quad\text{for every }x\in X,\qquad f(X):=\{f(x):x\in X\}\subseteq F(X).
$$

Here $f(X)$ means the actual [image of a function](image-of-a-function.md), also called its pointwise range on $X$; $F(X)$ denotes a calculated [interval enclosure](interval-enclosure.md). They need not agree. Sampling a few inputs can suggest a bound, but does not establish an [interval enclosure](interval-enclosure.md) between those inputs. Kearfott and coauthors explicitly distinguish the [image of a function](image-of-a-function.md) from evaluating an expression with [interval arithmetic](interval-arithmetic.md), because different expressions for the same [function](function-split.md) can give different bounds.[Kearfott, Nakao, Neumaier, Rump, Shary and Van Hentenryck, Standardized notation in interval analysis, 2010, Arithmetic expressions and Intervals and boxes](https://www.tuhh.de/ti3/paper/rump/KeNaNeRuShHe10.pdf)

## ↑ Ancestors (6)

1. [Interval arithmetic](interval-arithmetic.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Interval arithmetic](interval-arithmetic.md)
- [Interval arithmetic operations](interval-arithmetic-operations.md)
- [Interval bisection](interval-bisection.md)
- [Interval dependency problem](interval-dependency-problem.md)
- [Interval enclosure](interval-enclosure.md)
- [Interval root exclusion](interval-root-exclusion.md)
- [Interval subdivision](interval-subdivision.md)
- [Natural interval extension](natural-interval-extension.md)
- [Outward rounding](outward-rounding.md)
