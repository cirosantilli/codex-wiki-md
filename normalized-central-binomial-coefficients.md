# Normalized central binomial coefficients

↑ **Parent:** [Central binomial coefficient](central-binomial-coefficient.md)

Set $c_n=4^{-n}\binom{2n}{n}$, with $c_0=1$. Cancellation of factorials gives

$$
c_n=\prod_{j=1}^n\left(1-\frac1{2j}\right),\qquad
\frac{c_{n+1}}{c_n}=1-\frac1{2n+2}.
$$

Consequently $c_n$ decreases to zero: $\log c_n\leq-\frac12\sum_{j=1}^n1/j\leq-\frac12\log(n+1)$. The inequality uses $\log(1-x)\leq-x$ and comparison with $\int_1^{n+1}dt/t$. Conversely $c_n\geq1/(n+1)$ by induction, since its ratio is at least $(n+1)/(n+2)$. Thus $\sum c_n$ diverges while $\sum(-1)^nc_n$ has [conditional convergence](conditional-convergence.md) by the [alternating series test](alternating-series-test.md). These elementary bounds require no asymptotic formula for factorials.

## ↑ Ancestors (6)

1. [Central binomial coefficient](central-binomial-coefficient.md)
2. [Binomial coefficient](binomial-coefficient.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1/12f/ii/solution.md)
