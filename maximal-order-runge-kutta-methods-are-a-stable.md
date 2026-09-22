# Maximal-order Runge-Kutta methods are A-stable

↑ **Parent:** [Runge-Kutta method](runge-kutta-method.md)

An $s$-stage [Runge-Kutta method](runge-kutta-method.md) has [stability function](stability-function.md) $R(z)=1+zb^T(I-zA)^{-1}\mathbf1$, a [rational function](rational-function.md) with numerator and denominator degrees at most $s$. Order $2s$ forces $R(z)-e^z=O(z^{2s+1})$, so uniqueness of the diagonal [Padé approximant](pade-approximant.md) identifies $R$ with $[s/s]_{e^z}$. That approximant has no poles in the closed left half-plane and modulus at most one there. Hence every such maximal-order method is [A-stable](a-stability.md). Since the [Padé approximant](pade-approximant.md) numerator and denominator are coprime and both have degree $s$, the original stage [determinant](determinant.md) cannot have hidden canceled poles in that half-plane.

## ↑ Ancestors (6)

1. [Runge-Kutta method](runge-kutta-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/1/a/solution.md)
