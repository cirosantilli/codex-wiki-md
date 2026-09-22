<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Substitution of $y=x^p$ into the homogeneous [Euler-Cauchy equation](../../../../euler-cauchy-equation.md) gives $(p(p-1)+p-1)x^{p-2}=(p^2-1)x^{p-2}$, so $\boxed{p=1,-1}$. Use the solution $u(x)=x$ that vanishes at zero and $v(x)=1/x$ that decays at infinity. Their [Wronskian](../../../../wronskian.md) is $uv'-u'v=-2/x$. The [half-line Green function for the first cylindrical harmonic](../../../../half-line-green-function-for-the-first-cylindrical-harmonic.md) is therefore

$$
\boxed{G(x,s)=\begin{cases}-x/2,&0<x\leq s,\\-s^2/(2x),&0<s\leq x.\end{cases}}
$$

It is continuous at $x=s$, its first [derivative](../../../../derivative.md) has jump $1/2-(-1/2)=1$, and it solves the homogeneous equation elsewhere. Thus $L_xG=\delta(x-s)$ for integration with ordinary measure $ds$. The [boundary conditions](../../../../boundary-condition.md) hold for each fixed $s>0$.

Integrating against the forcing gives

$$
y(x)=-\frac1{2x}\int_0^xs^2e^{-s}ds-\frac x2\int_x^\infty e^{-s}ds.
$$

Since the two [integrals](../../../../integral-split.md) are $2-(x^2+2x+2)e^{-x}$ and $e^{-x}$, respectively,

$$
\boxed{y(x)=\frac{(x+1)e^{-x}-1}{x}\quad(x>0),\qquad y(0)=0.}
$$

A [Taylor expansion](../../../../taylor-expansion.md) gives $y=-x/2+O(x^2)$ near zero, while $y\sim-1/x$ at infinity. This verifies the two endpoint limits; direct differentiation verifies $Ly=e^{-x}$ on $x>0$. The differential expression itself is singular at zero, so the endpoint condition is imposed by continuity. No nonzero combination of $x$ and $1/x$ satisfies both homogeneous endpoint conditions, proving [uniqueness](../../../../uniqueness.md).

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
