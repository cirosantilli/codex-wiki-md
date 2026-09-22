<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

In monic form the [Chebyshev differential equation](../../../../chebyshev-differential-equation.md) has $P(x)=-x/(1-x^2)$ and $Q(x)=p^2/(1-x^2)$. Both are analytic near zero, so it is an [ordinary point](../../../../ordinary-point-criterion-for-a-second-order-equation.md). At $x=1$, $(x-1)P=x/(x+1)$ and $(x-1)^2Q=-p^2(x-1)/(x+1)$ are analytic; at $x=-1$, $(x+1)P=x/(x-1)$ and $(x+1)^2Q=-p^2(x+1)/(x-1)$ are analytic. Thus both endpoints are [regular singular points](../../../../regular-singular-point.md).

Insert $y_q=\sum_{n\geq0}a_nx^{n+q}$ and equate coefficients. The [recurrence relation](../../../../recurrence-relation.md) is

$$
\boxed{a_{n+2}=\frac{(n+q)^2-p^2}{(n+q+2)(n+q+1)}a_n,\qquad q=0,1.}
$$

Explicitly the factors are $(n^2-p^2)/[(n+2)(n+1)]$ for $q=0$ and $[(n+1)^2-p^2]/[(n+3)(n+2)]$ for $q=1$. The lowest equation for $q=1$ forces $a_1=0$. For $q=0$, one may choose $a_1=0$ to select an even solution, independent of the odd $q=1$ solution. The leading coefficient $a_0$ is free in either chosen parity branch.

For a nonterminating branch the consecutive parity-term ratio tends to $x^2$. Hence the [ratio test](../../../../ratio-test.md) gives convergence for $|x|<1$, and [radius of convergence](../../../../radius-of-convergence.md) one. Terminating branches are [polynomials](../../../../polynomial-split.md) with infinite radius. For $p=m\geq0$ an integer, choose $q$ of the same parity as $m$: the recurrence stops once $n+q=m$, producing a degree-$m$ [Chebyshev polynomial](../../../../chebyshev-polynomial.md). Normalization at $1$ gives all nonzero coefficients through degree three:

$$
\boxed{T_0=1,\qquad T_1=x,\qquad T_2=2x^2-1,\qquad T_3=4x^3-3x.}
$$

Set $Y(\theta)=y(\cos\theta)$. Direct [differentiation](../../../../differentiation.md) gives $Y''=\sin^2\theta\,y''-\cos\theta\,y'$, so the equation becomes $Y''+m^2Y=0$. For $m>0$, $Y=A\cos(m\theta)+B\sin(m\theta)$. A [polynomial](../../../../polynomial-split.md) $y$ has finite [derivative](../../../../derivative.md) at $x=1$, and therefore $Y'(0)=-\sin0\,y'(1)=0$, forcing $B=0$. Also $Y(0)=T_m(1)=1$, so $A=1$. For $m=0$, the transformed solution is affine in $\theta$ and the same [derivative](../../../../derivative.md) condition removes its linear term. Thus

$$
\boxed{T_m(x)=\cos(m\arccos x),\qquad -1\leq x\leq1,\quad m=0,1,2,\ldots.}
$$

The endpoint values follow by continuity. The finite-derivative condition is what excludes the independent nonpolynomial branch, rather than normalization alone.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
