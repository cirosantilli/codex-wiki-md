# Chebyshev nodal derivative comparison

↑ **Parent:** [Chebyshev polynomial](chebyshev-polynomial.md)

Let $x_j=\cos((2j-1)\pi/(2n))$ be the roots of the [Chebyshev polynomial](chebyshev-polynomial.md), and let $q$ have degree at most $n-1$ with $|q(x_j)|\le |T_n'(x_j)|$. Its [Lagrange interpolation polynomial](lagrange-polynomial.md) uses basis $\ell_j(x)=T_n(x)/[(x-x_j)T_n'(x_j)]$. For $x>x_1$, $T_n(x)>0$ and $x-x_j>0$, so $\ell_j(x)T_n'(x_j)>0$. Therefore $|q(x)|\le\sum_j|\ell_j(x)T_n'(x_j)|=T_n'(x)$, the last equality being interpolation of the derivative. Continuity includes $x=x_1$ and reflection proves the left-hand region.

## ↑ Ancestors (6)

1. [Chebyshev polynomial](chebyshev-polynomial.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bernstein inequality for algebraic polynomials](bernstein-inequality-for-algebraic-polynomials.md)
- [Markov inequality for polynomial derivatives](markov-inequality-for-polynomial-derivatives.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62/3/a/solution.md)
