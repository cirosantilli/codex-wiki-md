# Rounded Bernstein polynomial

↑ **Parent:** [Bernstein polynomial](bernstein-polynomial.md)

The rounded [Bernstein polynomial](bernstein-polynomial.md) replaces each coefficient $\binom nk f(k/n)$ in the unnormalized [basis](basis.md) $x^k(1-x)^{n-k}$ by its [floor function](floor-function.md). It therefore has [integer](integer.md) [coefficients](coefficient.md) in the ordinary monomial [basis](basis.md). If $f(0),f(1)\in\mathbb Z$, only interior rounding errors remain and

$$
\|B_n^*f-B_nf\|_\infty\le\max\{3/(2n),(n-1)(3/4)^n\}\longrightarrow0\qquad(n\ge2).
$$

To prove this, bound each interior rounding error by one. On $[0,1/4]$, sum the resulting powers as a [geometric series](geometric-series.md) of ratio at most $1/3$ and maximize $x(1-x)^{n-1}$; reflect for $[3/4,1]$. On the middle interval each degree-$n$ product is at most $(3/4)^n$. [integer](integer.md) endpoints are necessary for this convergence: a noninteger endpoint produces a fixed nonzero rounding error there.

## ↑ Ancestors (8)

1. [Bernstein polynomial](bernstein-polynomial.md)
2. [Weierstrass approximation theorem](weierstrass-approximation-theorem.md)
3. [Stone-Weierstrass theorem](stone-weierstrass-theorem.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Integer-coefficient polynomial approximation](integer-coefficient-polynomial-approximation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/2/b/solution.md)
