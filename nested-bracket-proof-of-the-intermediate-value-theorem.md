# Nested-bracket proof of the intermediate value theorem

↑ **Parent:** [Intermediate value theorem](intermediate-value-theorem.md)

For a short proof outline, endpoint values give the non-strict cases immediately. If $y$ is strictly between $f(a)$ and $f(b)$, apply the [bisection method](bisection-method.md) to the [continuous function](continuous-function.md) $g(x)=f(x)-y$. A [midpoint](midpoint.md) with $g=0$ finishes the proof. Otherwise retain [nested intervals](nested-intervals.md) $[a_k,b_k]$ with strictly opposite signs and widths $(b-a)2^{-k}$. The [nested interval theorem](nested-interval-theorem.md), using [completeness of the real numbers](completeness-of-the-real-numbers.md), gives a common point $c$ to which both endpoint [sequences](sequence.md) converge. After reversing the sign of $g$ if necessary, $g(a_k)<0<g(b_k)$. [Continuity](continuous-function.md) makes both endpoint value [sequences](sequence.md) converge to $g(c)$, forcing $g(c)\leq0$ and $g(c)\geq0$, hence $f(c)=y$. The original endpoint values differ from $y$, so $c\in(a,b)$. This proof explains why a jump can defeat the construction: shrinking a candidate [closed interval](closed-real-interval.md) cannot supply the missing [continuity](continuous-function.md).

## ↑ Ancestors (9)

1. [Intermediate value theorem](intermediate-value-theorem.md)
2. [Continuous function](continuous-function.md)
3. [Limit of a function](limit-of-a-function.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
