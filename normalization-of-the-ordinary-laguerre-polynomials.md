# Normalization of the ordinary Laguerre polynomials

↑ **Parent:** [Laguerre polynomial](laguerre-polynomial.md)

The [Laguerre polynomial](laguerre-polynomial.md) normalized by $L_n(0)=1$ has coefficients $L_n(x)=\sum_{j=0}^n(-1)^j\binom njx^j/j!$. By the [Leibniz rule](leibniz-rule.md), this is equivalent to [Rodrigues' formula](rodrigues-formula.md), $e^{-x}L_n(x)=D^n(e^{-x}x^n)/n!$. For any [polynomial](polynomial-split.md) $q$ of degree below $n$, $n$ applications of [integration by parts](integration-by-parts.md) give $\int_0^\infty e^{-x}L_nq\,dx=0$. All endpoint terms vanish: derivatives of $e^{-x}x^n$ of order below $n$ vanish at zero and decay at infinity. Since $L_n^{(n)}=(-1)^n$, the same calculation gives

$$
\int_0^\infty e^{-x}L_n^2\,dx
=\frac{(-1)^n}{n!}\int_0^\infty e^{-x}x^nL_n^{(n)}\,dx
=\frac{\Gamma(n+1)}{n!}=1.
$$

Thus these [orthogonal polynomials](orthogonal-polynomial-split.md) are already an [orthonormal set](orthonormal-set.md) for the [weighted inner product](weighted-inner-product.md) with weight $e^{-x}$.

## ↑ Ancestors (9)

1. [Laguerre polynomial](laguerre-polynomial.md)
2. [Laguerre differential operator on polynomials](laguerre-differential-operator-on-polynomials.md)
3. [Self-adjoint operator](self-adjoint-operator.md)
4. [Operator theory](linear-operator-theory-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-2/1/d/solution.md)
