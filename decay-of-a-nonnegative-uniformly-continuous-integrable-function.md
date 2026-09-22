# Decay of a nonnegative uniformly continuous integrable function

↑ **Parent:** [Uniformly continuous function](uniformly-continuous-function.md)

A [nonnegative function](nonnegative-function.md) that is a [uniformly continuous function](uniformly-continuous-function.md) on the [interval](interval-mathematics.md) $[0,\infty)$ and has a finite [integral](integral-split.md) tends to zero. Otherwise [uniform continuity](uniform-continuity.md) gives disjoint [intervals](interval-mathematics.md) of a fixed width on which the [function](function-split.md) exceeds a fixed positive value, contradicting [integrability](integrability.md). This supplies a useful decay argument for [Lyapunov functions](lyapunov-function.md) with merely [continuous](continuous-function.md) [vector fields](vector-field.md).

To make the fixed width explicit, suppose some $\eta>0$ occurs as a lower bound $f(t_n)\geq\eta$ along a [sequence](sequence.md) with $t_n\to\infty$. Choose $\delta>0$ from [uniform continuity](uniform-continuity.md) for output tolerance $\eta/2$. On every [interval](interval-mathematics.md) $(t_n-\delta/2,t_n+\delta/2)$ lying in $[0,\infty)$, the [function](function-split.md) is greater than $\eta/2$. Extract a [subsequence](subsequence.md) whose centers are more than $\delta$ apart. Each disjoint [interval](interval-mathematics.md) contributes at least $\eta\delta/2$ to the [integral](integral-split.md), so the first $N$ contribute at least $N\eta\delta/2$. This contradicts finiteness of the [integral](integral-split.md). The same input width at every center is the essential step; [continuity](continuous-function.md) alone would allow progressively narrower peaks.

## ↑ Ancestors (9)

1. [Uniformly continuous function](uniformly-continuous-function.md)
2. [Continuous function](continuous-function.md)
3. [Limit of a function](limit-of-a-function.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213/4/solution.md)
