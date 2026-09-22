<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [Runge-Kutta method](../../../../../../runge-kutta-method.md) to the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md) and put $z=h\lambda$. Its [stability function](../../../../../../stability-function.md) is

$$
R(z)=1+z\,b^T(I-zA)^{-1}\mathbf1=\frac{P(z)}{Q(z)},\qquad Q(z)=\det(I-zA).
$$

Since $A$ is an [invertible matrix](../../../../../../invertible-matrix.md), $Q$ has [polynomial degree](../../../../../../degree-of-a-polynomial.md) $s$. The [adjugate matrix](../../../../../../adjugate-matrix.md) formula gives $\deg P\le s$, but the additional condition gives

$$
\lim_{z\to\infty}R(z)=1-b^TA^{-1}\mathbf1=0,
$$

so actually $\deg P\le s-1$. The specified [order of a numerical method](../../../../../../order-of-a-numerical-method.md) implies $R(z)=e^z+O(z^{2s})$ near zero. Therefore the [Padé identification of a Radau stability function](../../../../../../pade-identification-of-a-radau-stability-function.md) makes $R$ the $[s-1/s]$ [Padé approximant](../../../../../../pade-approximant.md) to the [exponential function](../../../../../../exponential-function.md): its numerator and denominator have the required degrees, and its [Taylor series](../../../../../../taylor-series.md) agrees through degree $2s-1$.

In the permitted [A-stability of near-diagonal exponential Padé approximants](../../../../../../a-stability-of-near-diagonal-exponential-pade-approximants.md), take $m=s-1$, $n=s$. Then $n-2\le m\le n$, so **the scheme is [A-stable](../../../../../../a-stability.md)**. The same [stability function](../../../../../../stability-function.md) also tends to zero at infinity, giving [L-stability](../../../../../../l-stability.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
