# Interval root exclusion

↑ **Parent:** [Interval arithmetic](interval-arithmetic.md)

[Interval root exclusion](interval-root-exclusion.md) certifies that a [function](function-split.md) has no [zero of a function](zero-of-a-function.md) on $X$ when a valid [interval enclosure](interval-enclosure.md) $F(X)$ excludes zero. For $g(x)=x(1-x)-1/3$ on $[0,1]$, the [interval square range](interval-square-range.md) yields $G(X)=[-1/3,-1/12]$, which excludes zero. Direct [interval arithmetic](interval-arithmetic.md) yields $[-1/3,2/3]$ and is inconclusive, even though the [function](function-split.md) has no [zero of a function](zero-of-a-function.md) there.

Knowing only that a calculated [interval enclosure](interval-enclosure.md) contains zero does not certify a [zero of a function](zero-of-a-function.md): it may contain unattainable values. Even the positive [constant function](constant-function.md) $f(x)=1$ has a valid, loose [interval enclosure](interval-enclosure.md) $[-1,2]$. A separate existence argument, such as reliable opposite endpoint signs together with [continuity](continuous-function.md) in the [intermediate value theorem](intermediate-value-theorem.md), is required; see [root bracket](root-bracket.md) and [bisection method](bisection-method.md). [Interval subdivision](interval-subdivision.md) can resolve some inconclusive pieces, but remaining pieces must be reported as unresolved unless an existence argument succeeds. This makes [interval root exclusion](interval-root-exclusion.md) useful for systematically discarding regions in a search.

// Target: analysis.bigb

## ↑ Ancestors (6)

1. [Interval arithmetic](interval-arithmetic.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Interval root exclusion](interval-root-exclusion.md)
