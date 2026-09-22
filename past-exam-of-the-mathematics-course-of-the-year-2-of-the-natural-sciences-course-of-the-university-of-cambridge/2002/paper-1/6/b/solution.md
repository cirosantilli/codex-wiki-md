<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $M=|m|$ for integer $m$. In the even or odd [power series](../../../../../power-series.md) whose parity matches $M$, the numerator in the [recurrence relation](../../../../../recurrence-relation.md) vanishes at the coefficient of $x^M$. All coefficients of lower powers in that parity are nonzero, and all higher ones vanish. Therefore a [polynomial](../../../../../polynomial-split.md) solution exists, of [polynomial degree](../../../../../degree-of-a-polynomial.md) $M$, containing

$$
\boxed{\left\lfloor\frac M2\right\rfloor+1\text{ nonzero terms}.}
$$

For nonnegative $m$ these are the [Chebyshev polynomials](../../../../../chebyshev-polynomial.md) $T_m$. The normalized low-degree cases follow directly from the [recurrence relation](../../../../../recurrence-relation.md):

$$
\begin{aligned}
m=0:&\quad y=a_0,\\
m=1:&\quad y=a_1x,\\
m=2:&\quad y=a_0(1-2x^2),\\
m=3:&\quad y=a_1(x-\tfrac43x^3).
\end{aligned}
$$

Enforcing $T_m(1)=1$ gives

$$
\boxed{T_0=1,\qquad T_1=x,\qquad T_2=2x^2-1,\qquad T_3=4x^3-3x.}
$$

To see that normalization at one is always possible, set $x=\cos\theta$ in the [Chebyshev differential equation](../../../../../chebyshev-differential-equation.md). For $Y(\theta)=y(\cos\theta)$, the differential expression $(1-x^2)y''-xy'$ becomes $Y''$. Thus $Y=\cos(M\theta)$ gives $T_M(x)=\cos(M\arccos x)$ on $[-1,1]$ and has value one at $x=1$. It is a [polynomial](../../../../../polynomial-split.md) because the [cosine addition formula](../../../../../cosine-addition-formula.md) gives $T_{M+1}=2xT_M-T_{M-1}$. Negative integer $m$ produces the same solution as $M=|m|$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
