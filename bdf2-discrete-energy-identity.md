# BDF2 discrete energy identity

↑ **Parent:** [Backward differentiation formula](backward-differentiation-formula.md)

For three [vectors](vector.md) $a,b,c$ in an [inner product space](inner-product-space.md), expansion of each squared [norm](norm.md) proves

$$
2\operatorname{Re}\langle3a-4b+c,a\rangle
=\|a\|^2+\|2a-b\|^2-\|b\|^2-\|2b-c\|^2+\|a-2b+c\|^2.
$$

Therefore the second-order [backward differentiation formula](backward-differentiation-formula.md) $3U^{n+2}-4U^{n+1}+U^n=2kLU^{n+2}$ with a [dissipative operator](dissipative-operator.md) $L$ decreases the discrete [energy](energy.md) $\mathcal E_n=\|U^{n+1}\|^2+\|2U^{n+1}-U^n\|^2$. This [quadratic form](quadratic-form.md) is equivalent to the product [norm](norm.md) of the two time levels with constants independent of $k$ and $L$. It proves uniform [stability](stability-of-a-numerical-method.md) even when amplification [roots of a polynomial](root-of-a-polynomial.md) coalesce inside the unit disk, where an eigenvector-separation proof may lose its bound.

## ↑ Ancestors (6)

1. [Backward differentiation formula](backward-differentiation-formula.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/7/solution.md)
- [Stability of a spatially shifted BDF2 stencil](stability-of-a-spatially-shifted-bdf2-stencil.md)
