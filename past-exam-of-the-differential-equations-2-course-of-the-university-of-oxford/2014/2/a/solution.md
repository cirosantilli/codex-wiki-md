<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work first on $0<x<1$. Divide by $x-1$ to put the equation in leading-coefficient-one form. Its first-derivative coefficient is $-x/(x-1)$, so the [integrating factor](../../../../integrating-factor.md) for the [self-adjoint differential operator](../../../../self-adjoint-differential-operator.md) is

$$
p(x)=\exp\left(\int\frac{-x}{x-1}\,dx\right)=\frac{e^{-x}}{1-x}.
$$

The resulting coefficients are

$$
\boxed{p(x)=\frac{e^{-x}}{1-x},\qquad q(x)=-\frac{e^{-x}}{(1-x)^2},\qquad
F(x)=-\frac{e^{-x}}{(1-x)^2}.}
$$

Indeed $p'(x)=x e^{-x}/(1-x)^2$, and multiplying the original equation by $-e^{-x}/(1-x)^2$ gives $(py')'+qy=F$. These transformed coefficients are singular at the right endpoint; the boundary value there is understood as the endpoint limit.

Substituting $y=x$ and $y=e^x$ in the homogeneous original equation gives zero in both cases. Their [Wronskian](../../../../wronskian.md) is

$$
W(x,e^x)=xe^x-e^x=(x-1)e^x,
$$

which is nonzero for $0<x<1$. Thus they are [linearly independent](../../../../linear-independence.md) on the solution interval.

To construct a [Dirichlet Green function](../../../../dirichlet-green-function.md), choose homogeneous solutions adapted to the two endpoints:

$$
u(x)=x,\qquad v(x)=e^x-ex,\qquad u(0)=0,\quad v(1)=0.
$$

Their [Wronskian](../../../../wronskian.md) is again $(x-1)e^x$, and $pW=-1$. Therefore the Green function for $L=(p\,d/dx)'+q$ with zero endpoint values is

$$
\boxed{G(x,s)=-u(\min(x,s))v(\max(x,s))
=\begin{cases}-x(e^s-es),&x\leq s,\\-s(e^x-ex),&s\leq x.\end{cases}}
$$

For fixed $s\in(0,1)$ it is continuous in $x$, vanishes at both endpoints, and satisfies the unit-flux jump condition

$$
p(s)\bigl[G_x(s^+,s)-G_x(s^-,s)\bigr]=1.
$$

Consequently $L_xG(x,s)=\delta(x-s)$ in the sense of [distributions](../../../../distribution-mathematical-analysis.md). This is a [singular-endpoint Green function with a double-zero right solution](../../../../singular-endpoint-green-function-with-a-double-zero-right-solution.md).

The endpoint data are nonhomogeneous, so use the homogeneous lifting $2x$ and write

$$
y(x)=2x+\int_0^1G(x,s)F(s)\,ds.
$$

Although $F(s)$ is singular at one, the integral exists for each interior $x$: the right solution satisfies $v(s)\sim e(1-s)^2/2$, cancelling the $(1-s)^{-2}$ forcing when $s>x$.

Splitting the integral at $s=x$ gives

$$
y(x)=2x+v(x)I_1(x)+xI_2(x),
$$

where elementary antiderivatives yield

$$
I_1(x)=\int_0^x\frac{s e^{-s}}{(1-s)^2}\,ds=\frac{e^{-x}}{1-x}-1,
$$



$$
I_2(x)=\int_x^1\frac{(e^s-es)e^{-s}}{(1-s)^2}\,ds
=\frac{e^{1-x}-1}{1-x}-1.
$$

For the second equality, an antiderivative is $(1-e^{1-s})/(1-s)$, whose endpoint limit at one is $-1$. Simplifying the Green representation gives

$$
\boxed{y(x)=1+(1+e)x-e^x.}
$$

It has the prescribed endpoint values. Direct substitution gives $(x-1)y''-xy'+y=1$, and at the degenerate endpoint it also obeys $-y'(1)+y(1)=1$. The only homogeneous solution satisfying both zero endpoint conditions is zero, so this solution is unique in the corresponding classical class.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
