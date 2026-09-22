# Coefficient sign lemma for the first Dahlquist barrier

↑ **Parent:** [Cayley coefficient proof of the first Dahlquist barrier](cayley-coefficient-proof-of-the-first-dahlquist-barrier.md)

Write $F(x)=\int_0^1(1+x)^t(1-x)^{1-t}\,dt=x/\operatorname{arctanh}x$. Pairing $t$ and $1-t$ after differentiating twice gives

$$
F''(x)=-4\int_0^1t(1-t)(1-x^2)^{-3/2}\cosh[(2t-1)\operatorname{arctanh}x]\,dt.
$$

The [power series](power-series.md) of $(1-x^2)^{-3/2}$ has strictly positive even coefficients, and the other factor has nonnegative even coefficients. Thus every even coefficient of $F''$ is negative. Since $F$ is even with $F(0)=1$, the displayed sign pattern follows. This supplies a short positivity argument for the [first Dahlquist barrier](first-dahlquist-barrier.md).

## ↑ Ancestors (8)

1. [Cayley coefficient proof of the first Dahlquist barrier](cayley-coefficient-proof-of-the-first-dahlquist-barrier.md)
2. [First Dahlquist barrier](first-dahlquist-barrier.md)
3. [Linear multistep method](linear-multistep-method.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/2/solution.md)
