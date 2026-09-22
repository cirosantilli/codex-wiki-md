<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $\Phi(r,\theta)=R(r)Y(\theta)$ in [Laplace's equation](../../../../laplace-equation.md), multiply by $r^2/(RY)$, and separate the two variables:

$$
\frac{(r^2R')'}R=-\frac{(\sin\theta\,Y')'}{Y\sin\theta}=\lambda.
$$

With $s=\cos\theta$, the angular equation becomes $(1-s^2)Y_{ss}-2sY_s+\lambda Y=0$. Requiring a smooth [axisymmetric harmonic function](../../../../axisymmetric-harmonic-function.md) at both poles selects $\lambda=n(n+1)$ and the [Legendre polynomial](../../../../legendre-polynomial.md) $Y=P_n(s)$, for nonnegative [integers](../../../../integer-split.md) $n$. The radial [Cauchy-Euler equation](../../../../cauchy-euler-equation.md) has solutions $r^n$ and $r^{-n-1}$. [Superposition](../../../../superposition-principle.md) over the angular [eigenfunctions](../../../../eigenfunction.md) therefore gives

$$
\Phi(r,\theta)=\sum_{n=0}^{\infty}(A_nr^n+B_nr^{-n-1})P_n(\cos\theta),\qquad (1-s^2)P_n''-2sP_n'+n(n+1)P_n=0.
$$

This expansion assumes regularity on each whole angular [sphere](../../../../sphere.md); without it, singular angular solutions would also be possible. The boundary data in the shell involve only the $n=0,1$ modes. Define the [spherical-shell harmonic interpolation](../../../../axisymmetric-harmonic-interpolation-between-concentric-spheres.md) weights

$$
p_0=\frac{a(b-r)}{r(b-a)},\quad q_0=\frac{b(r-a)}{r(b-a)},\qquad p_1=\frac{a^2(b^3-r^3)}{r^2(b^3-a^3)},\quad q_1=\frac{b^2(r^3-a^3)}{r^2(b^3-a^3)}.
$$

Each $p_n$ equals one at the inner boundary and zero at the outer one, and $q_n$ does the reverse. Hence the steady [temperature](../../../../temperature-split.md) is

$$
\boxed{T(r,\theta)=T_0p_0(r)+T_2q_0(r)+[T_1p_1(r)+T_3q_1(r)]\cos\theta.}
$$

Each term is a [harmonic function](../../../../harmonic-function.md), and substitution verifies both prescribed boundary values. Uniqueness follows from the [maximum principle for harmonic functions](../../../../maximum-principle-for-harmonic-functions.md).

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2007](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
