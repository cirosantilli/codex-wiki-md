# Laguerre orthonormality

↑ **Parent:** [Laguerre polynomial](laguerre-polynomial.md)

The ordinary [Laguerre polynomials](laguerre-polynomial.md), normalized by $L_n(0)=1$, are orthonormal for the weighted [inner product](inner-product-split.md) displayed above. Their coefficient formula is $L_n(x)=\sum_{k=0}^n(-1)^k\binom nkx^k/k!$. To prove the relation, use [Rodrigues' formula](rodrigues-formula.md) $e^{-x}L_n=(n!)^{-1}(x^ne^{-x})^{(n)}$ and integrate by parts $n$ times against $L_m$. For $n>m$ its $n$th derivative vanishes. At zero every derivative of $x^ne^{-x}$ of order less than $n$ vanishes, and at infinity the exponential kills every polynomial boundary term. For $n=m$, $L_n^{(n)}=(-1)^n$, so the integral is $(n!)^{-1}\int_0^\infty x^ne^{-x}\,dx=1$. Symmetry covers $m>n$. Thus these are orthonormal without an extra normalization factor.

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

- [Solution](past-exam-of-the-differential-equations-and-applications-course-of-the-university-of-oxford/2010/a/3/iii/solution.md)
