# Four-point midpoint third derivative

↑ **Parent:** [Finite difference](finite-difference-split.md)

The antisymmetric four-node stencil at offsets $-3h/2,-h/2,h/2,3h/2$ about a midpoint approximates the third [derivative](derivative.md). [Taylor expansion](taylor-expansion.md) gives leading error $h^2u^{(5)}/8$. For a third-order [boundary value problem](boundary-value-problem-split.md) on nodes $0,\ldots,n+1$, use rows $j=1,\ldots,n-1$, prescribed endpoint values and one consistent one-sided [derivative](derivative.md) condition. This avoids a ghost node while providing the correct number of equations. For instance a known right-endpoint first [derivative](derivative.md) is approximated by $(3U_{n+1}-4U_n+U_{n-1})/(2h)$.

## ↑ Ancestors (6)

1. [Finite difference](finite-difference-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2011/b/4/b/solution.md)
