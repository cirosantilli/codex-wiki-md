<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

**Adapted homogeneous solutions.** First assume real $\kappa\ne0$. The functions $u(x)=\cosh(\kappa x)$ and $v(x)=\cosh(\kappa(1-x))$ solve $z''-\kappa^2z=0$ and obey $u'(0)=v'(1)=0$. Their [Wronskian](../../../../wronskian.md) is

$$
W=uv'-u'v=-\kappa[\cosh(\kappa x)\sinh(\kappa(1-x))+\sinh(\kappa x)\cosh(\kappa(1-x))]=-\kappa\sinh\kappa.
$$

It is independent of $x$ and nonzero.

**Green function.** For $0<\xi<1$, continuity at $x=\xi$ and the jump condition $G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=1$ follow by matching the [Dirac delta function](../../../../dirac-delta-function.md) source. In particular a jump in $G$ itself would produce a derivative of the [Dirac delta function](../../../../dirac-delta-function.md), which is absent. Write $G=A(\xi)u(x)$ for $x<\xi$ and $G=B(\xi)v(x)$ for $x>\xi$. Solving the continuity and derivative-jump equations gives $A=v(\xi)/W$, $B=u(\xi)/W$. Hence the [Neumann Green function for the modified Helmholtz equation on an interval](../../../../neumann-green-function-for-the-modified-helmholtz-equation-on-an-interval.md) is

$$
\boxed{G(x,\xi)=-\frac1{\kappa\sinh\kappa}\begin{cases}\cosh(\kappa x)\cosh(\kappa(1-\xi)),&x\leq\xi,\\\cosh(\kappa\xi)\cosh(\kappa(1-x)),&x\geq\xi.\end{cases}}
$$

The two pieces coincide at the source. Their derivative difference is $W/W=1$ and their endpoint derivatives vanish. The same expression has continuous one-sided limits as the source approaches an endpoint; the interior-source construction is what is needed in the integral solution.

**Solution for a general source.** By [superposition](../../../../superposition-principle.md), $y(x)=\int_0^1G(x,\xi)f(\xi)\,d\xi$. Splitting the [integral](../../../../integral-split.md) at $\xi=x$ gives

$$
\boxed{y(x)=-\frac{\cosh(\kappa x)\displaystyle\int_x^1f(\xi)\cosh(\kappa(1-\xi))\,d\xi+\cosh(\kappa(1-x))\displaystyle\int_0^xf(\xi)\cosh(\kappa\xi)\,d\xi}{\kappa\sinh\kappa}.}
$$

No nonzero homogeneous solution satisfies both endpoint conditions when $\kappa\ne0$: the condition at zero eliminates $\sinh(\kappa x)$, and the condition at one then eliminates $\cosh(\kappa x)$. Thus the [Green function](../../../../green-s-function-split.md) gives the unique solution.

**The printed zero-parameter case.** The statement permits real $\kappa$, but $\kappa=0$ is exceptional. Integrating a putative equation $G''=\delta(x-\xi)$ would give $G'(1)-G'(0)=1$, contrary to the two zero derivatives. Thus this [Green function](../../../../green-s-function-split.md) does not exist at zero. For $y''=f$ with homogeneous [Neumann boundary conditions](../../../../neumann-boundary-condition.md), solvability instead requires $\int_0^1f=0$, and a compatible solution has an arbitrary additive constant. This is the [Fredholm solvability condition](../../../../fredholm-solvability-condition.md) associated with the constant zero mode.

**Explicit forcing.** For $f(x)=x$ and $\kappa=1$, the particular solution is $-x$. Write $y=C\cosh x+D\sinh x-x$. Then $y'(0)=0$ gives $D=1$ and $y'(1)=0$ gives $C=(1-\cosh1)/\sinh1=-\tanh(1/2)$. Therefore

$$
\boxed{y(x)=\sinh x-\tanh(1/2)\cosh x-x=\frac{\sinh(x-1/2)}{\cosh(1/2)}-x.}
$$

Direct differentiation gives $y'=\cosh(x-1/2)/\cosh(1/2)-1$, which vanishes at both endpoints, and $y''-y=x$, verifying the solution independently of the [Green function](../../../../green-s-function-split.md) integration.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
