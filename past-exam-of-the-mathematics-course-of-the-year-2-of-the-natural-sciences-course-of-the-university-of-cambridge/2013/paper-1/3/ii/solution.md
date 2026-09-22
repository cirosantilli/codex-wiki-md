<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the boundary-adapted [homogeneous solutions](../../../../../homogeneous-solution.md)

$$
u(x)=1+x,\qquad v(x)=e^x-\frac e2(1+x),\qquad W(x)=uv'-u'v=xe^x.
$$

For a source point $\xi\ne0$, the [Green function](../../../../../green-s-function-split.md) is

$$
\boxed{G(x,\xi)=\frac1{\xi e^\xi}\begin{cases}u(x)v(\xi),&x\leq\xi,\\u(\xi)v(x),&x\geq\xi.\end{cases}}
$$

It vanishes at both endpoints and is continuous at $x=\xi$. Its first [derivative](../../../../../derivative.md) has the jump

$$
G_x(\xi^+,\xi)-G_x(\xi^-,\xi)=\frac{u(\xi)v'(\xi)-u'(\xi)v(\xi)}{W(\xi)}=1,
$$

as required for a monic second-order [differential operator](../../../../../differential-operator.md) with a [Dirac delta](../../../../../dirac-delta-function.md) source. Away from that source it is a [homogeneous solution](../../../../../homogeneous-solution.md) and extends smoothly through $x=0$.

**The interior singular point requires a qualification.** This is a [Green kernel with a vanishing Wronskian at an interior singular point](../../../../../green-kernel-with-a-vanishing-wronskian-at-an-interior-singular-point.md), with a $1/\xi$ singularity in its source variable. It is not an ordinary integral inverse for unrestricted forcing. For smooth forcing $f(\xi)=\xi q(\xi)$, however, the product $Gf$ extends continuously at zero and the integral is well defined. This includes part (iii). We use solutions with two continuous derivatives across zero, interpreting the equation there after multiplication by $x$. For such a solution, expansion at zero forces $f(0)=0$; arbitrary nonzero forcing at zero cannot satisfy this regularity. Merely imposing one continuous derivative would leave a piecewise homogeneous ambiguity, so the original singular coefficients alone do not specify an unrestricted boundary-value inverse.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
