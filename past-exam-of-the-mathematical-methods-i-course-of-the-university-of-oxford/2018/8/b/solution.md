<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Substitute the [power series](../../../../power-series.md) and its termwise [derivatives](../../../../derivative.md) into the [ordinary differential equation](../../../../ordinary-differential-equation.md). The coefficient of $x^n$, for $n\geq0$, is

$$
(n+2)(n+1)a_{n+2}+[n(n-1)-6n+12]a_n=0.
$$

The bracket factors as $(n-3)(n-4)$, so the [power-series solution of a differential equation](../../../../power-series-solution-of-a-differential-equation.md) satisfies

$$
\boxed{a_{n+2}=-\frac{(n-3)(n-4)}{(n+1)(n+2)}a_n.}
$$

The odd and even [recurrence relations](../../../../recurrence-relation.md) terminate: $a_3=-a_1$, $a_5=0$, and $a_2=-6a_0$, $a_4=a_0$, $a_6=0$. Thus the full solution is $y=a_0(1-6x^2+x^4)+a_1(x-x^3)$. The two [polynomials](../../../../polynomial-split.md) have independent initial data at zero, and the leading coefficient $1+x^2$ never vanishes on the real axis, so every real [solution of a differential equation](../../../../solution-of-a-differential-equation.md) for this equation is their [linear combination](../../../../linear-combination.md) on the entire real axis. The given initial data select $a_0=0$, $a_1=1$:

$$
\boxed{y(x)=x-x^3.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
