<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Applying the [implicit midpoint rule](../../../../implicit-midpoint-rule.md) to the [simple harmonic oscillator](../../../../simple-harmonic-motion.md) system gives

$$
y_{n+1}-y_n=\frac h2(z_{n+1}+z_n),\qquad
z_{n+1}-z_n=-\frac h2(y_{n+1}+y_n).
$$

Factor the change in the [quadratic form](../../../../quadratic-form-split.md) $y^2+z^2$ and substitute these equations:

$$
\begin{aligned}
&(y_{n+1}^2+z_{n+1}^2)-(y_n^2+z_n^2)\\
&=(y_{n+1}-y_n)(y_{n+1}+y_n)
+(z_{n+1}-z_n)(z_{n+1}+z_n)\\
&=\frac h2(z_{n+1}+z_n)(y_{n+1}+y_n)
-\frac h2(y_{n+1}+y_n)(z_{n+1}+z_n)=0.
\end{aligned}
$$

Thus every step preserves the [first integral](../../../../first-integral.md)

$$
\boxed{y_{n+1}^2+z_{n+1}^2=y_n^2+z_n^2
=y_0^2+z_0^2.}
$$

For completeness, the implicit equations are solvable for every real $h$: putting $s=h/2$, their coefficient [matrix](../../../../matrix.md) has [determinant](../../../../determinant.md) $1+s^2>0$ and the update is

$$
\begin{pmatrix}y_{n+1}\\z_{n+1}\end{pmatrix}
=\frac1{1+s^2}
\begin{pmatrix}1-s^2&2s\\-2s&1-s^2\end{pmatrix}
\begin{pmatrix}y_n\\z_n\end{pmatrix}.
$$

This is an [orthogonal matrix](../../../../orthogonal-matrix.md), as follows from $(1-s^2)^2+4s^2=(1+s^2)^2$. It therefore preserves the [Euclidean norm](../../../../euclidean-norm.md), explaining geometrically the exact energy conservation. This is a concrete instance of [Runge-Kutta conservation of quadratic invariants](../../../../runge-kutta-conservation-of-quadratic-invariants.md). Preservation of the circle does not assert that the numerical and exact solutions have the same phase at a fixed nonzero step size.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
