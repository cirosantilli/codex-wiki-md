# Deriving the Laguerre equation from Rodrigues' formula

↑ **Parent:** [Laguerre polynomial](laguerre-polynomial.md)

Set $v=x^ne^{-x}$. Direct [differentiation](differentiation.md) gives $xv'=(n-x)v$. Apply the [Leibniz rule](leibniz-rule.md) to differentiate $n+1$ times:

$$
xv^{(n+2)}+(n+1)v^{(n+1)}
=(n-x)v^{(n+1)}-(n+1)v^{(n)}.
$$

Hence $xv^{(n+2)}+(x+1)v^{(n+1)}+(n+1)v^{(n)}=0$. By [Rodrigues' formula](rodrigues-formula.md), $v^{(n)}=n!e^{-x}L_n$, so the next two [derivatives](derivative.md) are $n!e^{-x}(L_n'-L_n)$ and $n!e^{-x}(L_n''-2L_n'+L_n)$. Substitution gives the displayed [Laguerre differential operator on polynomials](laguerre-differential-operator-on-polynomials.md) eigenvalue equation. This derivation also covers $n=0$.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/20/b/solution.md)
