<h1 id="differential-equations/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

If $Au+Bv=0$, evaluation at zero gives $A=0$ and differentiation at zero gives $B=0$. Thus the solutions are [linearly independent](../../../../linear-independence.md). For $w=uv'-u'v$,

$$
w'=uv''-u''v=-p(uv'-u'v)=-pw,\qquad w(0)=1,
$$

so $\boxed{w(x)=\exp(-\int_0^xp(s)\,ds)>0}$.

[Variation of parameters](../../../../variation-of-parameters.md) sets $y=A(x)u+B(x)v$ with $A'u+B'v=0$, $A'u'+B'v'=f$. Solving gives $A'=-vf/w$ and $B'=uf/w$. Zero integration constants enforce both [initial conditions](../../../../initial-condition.md). Therefore

$$
\boxed{y(x)=\int_0^x\frac{v(x)u(t)-u(x)v(t)}{w(t)}f(t)\,dt,\qquad K(x,t)=\frac{v(x)u(t)-u(x)v(t)}{w(t)}.}
$$

For fixed $t$, this [kernel](../../../../green-s-function-split.md) is a [linear combination](../../../../linear-combination.md) of homogeneous solutions, so $K_{xx}+pK_x+qK=0$. On the diagonal $K(t,t)=0$ and $K_x(t,t)=(v'(t)u(t)-u'(t)v(t))/w(t)=1$. Differentiating the integral twice now verifies the forced equation as well as $y(0)=y'(0)=0$. Standard uniqueness of the linear [initial-value problem](../../../../initial-value-problem.md) makes this the solution, for [continuous](../../../../continuous-function.md) $f$.

If $u,v$ have [period](../../../../periodic-function.md) $T>0$, their [derivatives](../../../../derivative.md) do also, hence $w$ is [periodic](../../../../periodic-function.md). The [kernel](../../../../green-s-function-split.md) is [periodic](../../../../periodic-function.md) in its first variable. With $f=v$, split the integral at $x$ and use this periodicity to get

$$
y(x+T)-y(x)=-u(x)\int_x^{x+T}\frac{v(t)^2}{w(t)}\,dt+v(x)\int_x^{x+T}\frac{u(t)v(t)}{w(t)}\,dt.
$$

At $x=0$, the right side is $-\int_0^T v(t)^2/w(t)\,dt<0$, because $w>0$ and $v'(0)=1$ ensures $v$ is not identically zero. Thus $\boxed{y(T)\ne y(0)}$, so $y$ cannot have [period](../../../../periodic-function.md) $T$. This direct sign argument also rules out any apparent cancellation between the two terms.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Differential Equations](../../differential-equations.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
