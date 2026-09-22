<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [product rule](../../../../../product-rule.md) gives $\psi'=e^{-x^2/2}(y'-xy)$ and $\psi''=e^{-x^2/2}[y''-2xy'+(x^2-1)y]$. Substituting in the [Schrödinger equation](../../../../../schrodinger-equation.md) cancels the $x^2$ and constant terms, leaving the [Hermite differential equation](../../../../../hermite-differential-equation.md)

$$
y''-2xy'+2\lambda y=0.
$$

For $y=\sum_{n\geq0}a_nx^n$, matching coefficients gives

$$
a_{n+2}=\frac{2(n-\lambda)}{(n+2)(n+1)}a_n.
$$

The [power series solutions of the Hermite differential equation](../../../../../power-series-solutions-of-the-hermite-differential-equation.md) split into independent [even](../../../../../even-function.md) and [odd](../../../../../odd-function.md) series. With initial data $(y(0),y'(0))=(1,0)$ and $(0,1)$, respectively, their first three terms are

$$
y_e=1-\lambda x^2+\frac{\lambda(\lambda-2)}6x^4+O(x^6),\qquad y_o=x+\frac{1-\lambda}{3}x^3+\frac{(1-\lambda)(3-\lambda)}{30}x^5+O(x^7).
$$

Each nonterminating parity series has infinite [radius of convergence](../../../../../radius-of-convergence.md): the ratio of successive terms of that parity has magnitude asymptotic to $2|x|^2/n$. Their initial data prove [linear independence](../../../../../linear-independence.md). If a coefficient shown vanishes at a special parameter, the recurrence supplies the terminating series instead.

A nonzero [polynomial](../../../../../polynomial-split.md) solution of degree $N$ requires $\lambda=N$, by its highest-degree term, and the recurrence then terminates the matching parity. Thus all possible values are $\lambda=0,1,2,\ldots$. Up to nonzero [scalar multiples](../../../../../scalar-multiple.md), the degree-at-most-three solutions are the [Hermite polynomials](../../../../../hermite-polynomial.md)

$$
\boxed{\begin{array}{c|c} \lambda&y\\\hline0&1\\1&2x\\2&4x^2-2\\3&8x^3-12x\end{array}.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
