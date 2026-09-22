# Expected value of a capped nonnegative random variable

↑ **Parent:** [Tail-sum formula](tail-sum-formula.md)

For a nonnegative [random variable](random-variable-split.md) $Y$ and a fixed cap $a\geq0$, the [tail-sum formula](tail-sum-formula.md) gives

$$
\mathbb E[\min(Y,a)]=\int_0^a\mathbb P(Y>t)dt,\qquad
\mathbb E[(Y-a)_+]=\int_a^\infty\mathbb P(Y>t)dt.
$$

Below the cap, the [events](event.md) $\{\min(Y,a)>t\}$ and $\{Y>t\}$ coincide; at and above the cap, the former [event](event.md) is empty. For the second identity, the [positive part](positive-part-of-a-real-valued-function.md) $(Y-a)_+$ exceeds $t\geq0$ precisely when $Y>a+t$. Thus the two [integrals](integral-split.md) divide the [area](surface-area.md) under the [survival function](survival-function.md), just as $Y=\min(Y,a)+(Y-a)_+$ divides each outcome. The capped [expected value](expected-value-split.md) is always finite, while the excess [expected value](expected-value-split.md) may be infinite.

For the [uniform distribution](continuous-uniform-distribution.md) on the [interval](interval-mathematics.md) $[0,4]$ and cap $a=2$, the capped [expected value](expected-value-split.md) is $\int_0^2(1-t/4)dt=3/2$ and the excess [expected value](expected-value-split.md) is $\int_2^4(1-t/4)dt=1/2$. Directly averaging the capped values also gives $\int_0^2y(1/4)dy+2\mathbb P(Y>2)=1/2+1=3/2$. Capping therefore measures a different average from the uncapped [expected value](expected-value-split.md) two, even when both are finite.

## ↑ Ancestors (7)

1. [Tail-sum formula](tail-sum-formula.md)
2. [Expected value](expected-value-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Tail-sum formula](tail-sum-formula.md)
