<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [Runge-Kutta method](../../../../../../runge-kutta-method.md) coefficients as $A\in\mathbb R^{\nu\times\nu}$, $b\in\mathbb R^\nu$, and let $e$ be the all-ones column. On the test equation $y'=\lambda y$, with $z=h\lambda$, the stage [vector](../../../../../../vector.md) satisfies $Y=ey_n+zAY$ and the next value is $y_{n+1}=y_n+zb^TY$. Hence its [stability function](../../../../../../stability-function.md) is

$$
R(z)=1+zb^T(I-zA)^{-1}e
=\frac{\det(I-zA+zeb^T)}{\det(I-zA)}.
$$

Both [polynomials](../../../../../../polynomial-split.md) have degree at most $\nu$, and the denominator has value one at zero. [Order of a Runge-Kutta method](../../../../../../order-of-a-runge-kutta-method.md) $2\nu$ implies that this test-equation approximation agrees with $e^z$ through degree $2\nu$:

$$
R(z)-e^z=O(z^{2\nu+1}).
$$

By uniqueness of the diagonal [Padé approximant](../../../../../../pade-approximant.md), $R=[\nu/\nu]_{e^z}$. Explicitly,

$$
R(z)=\frac{P_\nu(z)}{P_\nu(-z)},\qquad
P_\nu(z)=\sum_{j=0}^\nu\frac{(2\nu-j)!\,\nu!}{(2\nu)!\,j!\,(\nu-j)!}\,z^j.
$$

The permitted diagonal [Padé approximant](../../../../../../pade-approximant.md) property says this [rational function](../../../../../../rational-function.md) has no poles in the closed left half-plane and satisfies $|R(z)|\le1$ there. Therefore

$$
\boxed{\text{Every }\nu\text{-stage Runge-Kutta method of order }2\nu\text{ is A-stable}.}
$$

There is also no hidden stage-solve singularity from a canceled denominator: the [Padé approximant](../../../../../../pade-approximant.md) numerator and denominator are coprime and each has degree $\nu$. The original [determinant](../../../../../../determinant.md) denominator already has degree at most $\nu$, so, with its normalization at zero, it equals $P_\nu(-z)$ and cannot contain an additional canceled factor. This proves [maximal-order Runge-Kutta methods are A-stable](../../../../../../maximal-order-runge-kutta-methods-are-a-stable.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
