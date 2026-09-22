# Square-root logarithmic sum over primes

↑ **Parent:** [Mertens first theorem](mertens-first-theorem.md)

Put $A(t)=\sum_{p\le t}(\log p)/p$. The [Mertens first theorem](mertens-first-theorem.md) gives $A(t)=\log t+O(1)$. [Partial summation](abel-s-summation-formula.md) yields

$$
\sum_{p\le x}\frac{\sqrt{\log p}}p
=\frac{A(x)}{\sqrt{\log x}}+\frac12\int_2^x\frac{A(t)}{t(\log t)^{3/2}}\,dt.
$$

The main terms sum to $2\sqrt{\log x}$ up to a constant. The error integral is bounded because $\int_2^\infty dt/(t(\log t)^{3/2})$ converges. Thus a [prime sum](prime-sum.md) with a fractional logarithmic weight follows from an elementary bounded-error estimate, without the [Prime number theorem](prime-number-theorem.md).

## ↑ Ancestors (7)

1. [Mertens first theorem](mertens-first-theorem.md)
2. [Mertens' theorems](mertens-theorems.md)
3. [Analytic number theory](analytic-number-theory-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/1/solution.md)
