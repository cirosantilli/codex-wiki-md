# Chebyshev interpolation represents external evaluation

↑ **Parent:** [Chebyshev polynomial domination lemma](chebyshev-polynomial-domination-lemma.md)

On real polynomials of degree at most $n\geq1$ with the [uniform norm](supremum-norm.md) on $[-1,1]$, set $x_j=\cos(j\pi/n)$ and let $\ell_j$ be the [Lagrange interpolation](lagrange-polynomial.md) basis. If $u>1$, the denominator of $\ell_j(u)$ has exactly $j$ negative factors while its numerator is positive. Therefore $|\ell_j(u)|=(-1)^j\ell_j(u)$. Since $T_n(x_j)=(-1)^j$, interpolation gives $\sum_j|\ell_j(u)|=T_n(u)$. Hence $|P(u)|\leq\|P\|_\infty T_n(u)$, and $P=T_n$ attains equality. Reflection and Chebyshev parity give the case $u<-1$. Dividing the interpolation weights by $T_n(u)$ yields an exact signed evaluation representation of norm one on $n+1$ nodes. Constants give the immediate degree-zero case.

## ↑ Ancestors (7)

1. [Chebyshev polynomial domination lemma](chebyshev-polynomial-domination-lemma.md)
2. [Chebyshev polynomial](chebyshev-polynomial.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-6/4/solution.md)
