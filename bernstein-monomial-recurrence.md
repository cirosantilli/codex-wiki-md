# Bernstein monomial recurrence

↑ **Parent:** [Bernstein polynomial](bernstein-polynomial.md)

For $m\ge1$ and $n\ge2$, the [Bernstein polynomial](bernstein-polynomial.md) of the [monomial](monomial.md) $x^m$ satisfies

$$
B_n(x^m)=x\sum_{\ell=0}^{m-1}\binom{m-1}{\ell}\frac{(n-1)^{m-1-\ell}}{n^{m-1}}B_{n-1}(x^{m-1-\ell}).
$$

It follows by applying $k\binom nk=n\binom{n-1}{k-1}$ and expanding $k=(k-1)+1$ with the [binomial theorem](binomial-theorem.md). The coefficients sum to one; only the first tends to one as $n\to\infty$. Induction on $m$ proves [uniform convergence](uniform-convergence.md) of these monomial approximants, starting from $B_n(1)=1$.

## ↑ Ancestors (8)

1. [Bernstein polynomial](bernstein-polynomial.md)
2. [Weierstrass approximation theorem](weierstrass-approximation-theorem.md)
3. [Stone-Weierstrass theorem](stone-weierstrass-theorem.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/7d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/7d/b/solution.md)
