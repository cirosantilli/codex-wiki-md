<h1 id="pade-identification-of-a-radau-stability-function">Padé identification of a Radau stability function</h1>

↑ **Parent:** [Radau IIA method](radau-iia-method.md)

Suppose an $s$-stage [Runge-Kutta method](runge-kutta-method.md) has order $2s-1$, an [invertible matrix](invertible-matrix.md) $A$, and $b^TA^{-1}\mathbf1=1$. Its [stability function](stability-function.md) is $R(z)=1+zb^T(I-zA)^{-1}\mathbf1$. The [adjugate matrix](adjugate-matrix.md) formula gives a [rational function](rational-function.md) with denominator degree $s$ and numerator degree at most $s$; its zero [limit](limit-of-a-function.md) at infinity lowers the latter degree to at most $s-1$. The [order of a numerical method](order-of-a-numerical-method.md) gives $R(z)-e^z=O(z^{2s})$, identifying the $[s-1/s]$ [Padé approximant](pade-approximant.md). Uniqueness follows because the cross-multiplied difference of two candidates has degree at most $2s-1$ but a zero of order at least $2s$, so is identically zero. The [A-stability of near-diagonal exponential Padé approximants](a-stability-of-near-diagonal-exponential-pade-approximants.md) then proves [A-stability](a-stability.md), and the zero limit proves [L-stability](l-stability.md). These conditions identify the stability function; they do not alone claim uniqueness of all entries of the [Runge-Kutta method](runge-kutta-method.md) tableau.

## ↑ Ancestors (9)

1. [Radau IIA method](radau-iia-method.md)
2. [Collocation Runge-Kutta method](collocation-runge-kutta-method.md)
3. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
4. [Runge-Kutta method](runge-kutta-method.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/1/a/solution.md)
