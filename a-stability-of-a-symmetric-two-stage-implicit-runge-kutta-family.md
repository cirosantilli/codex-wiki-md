# A-stability of a symmetric two-stage implicit Runge-Kutta family

↑ **Parent:** [A-stability](a-stability.md)

For the two-stage [implicit Runge-Kutta method](implicit-runge-kutta-method.md) with

$$
A=
\begin{pmatrix}
\frac14&\frac14-a\\
\frac14+a&\frac14
\end{pmatrix},
\qquad
b=\begin{pmatrix}\frac12\\\frac12\end{pmatrix},
$$

the [stability function](stability-function.md) is

$$
R(z)=\frac{2+z+2a^2z^2}{2-z+2a^2z^2}.
$$

For $z=x+iy$,

$$
|2-z+2a^2z^2|^2-|2+z+2a^2z^2|^2
=-8x(1+a^2|z|^2).
$$

The denominator has no zero in the closed left half-plane, so the method is [A-stable](a-stability.md) for every real $a$.

## ↑ Ancestors (7)

1. [A-stability](a-stability.md)
2. [Linear stability domain](linear-stability-domain.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/38c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-2/17b/b/solution.md)
