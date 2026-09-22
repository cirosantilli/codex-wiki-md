<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret the [Dirac delta](../../../../../dirac-delta-function.md) coefficient as a [point interaction in a second-order differential equation](../../../../../point-interaction-in-a-second-order-differential-equation.md). The solution is continuous at $x=1$ and is twice differentiable on either side, where $y''=f$. Its [transmission conditions for a delta coefficient](../../../../../transmission-conditions-for-a-delta-coefficient.md) are

$$
[y]_1=0,\qquad [y']_1=-\alpha y(1).
$$

Indeed, the [distributional second derivative across a jump](../../../../../distributional-second-derivative-across-a-jump.md) contributes $[y']_1\delta(x-1)$, which must cancel the delta coefficient because $f$ has no point source.

Put $s=y'(0)$ and $F(x)=\int_0^x(x-t)f(t)\,dt$. Integrating the ordinary equation and inserting the required derivative jump gives

$$
y(x)=c_1+sx+F(x)-\alpha y(1)(x-1)_+,\qquad y(1)=c_1+s+F(1),
$$

where $(x-1)_+=\max(x-1,0)$. This formula is continuous, has the stated jump, satisfies the equation, and parametrizes every solution with the left endpoint value. Imposing the right endpoint value gives the scalar equation

$$
\bigl[\pi-\alpha(\pi-1)\bigr]s
=c_2-c_1-F(\pi)+\alpha(\pi-1)\bigl(c_1+F(1)\bigr).
$$

Consequently a unique $s$, and hence a unique solution for every $f,c_1,c_2$, exists precisely when

$$
\boxed{\alpha\ne\alpha_*:=\frac\pi{\pi-1}.}
$$

At the exceptional value, the nonzero homogeneous solution with zero endpoint values is

$$
\phi(x)=\begin{cases}x,&0\leq x\leq1,\\(\pi-x)/(\pi-1),&1\leq x\leq\pi.\end{cases}
$$

It has derivative jump $-\pi/(\pi-1)=-\alpha_*\phi(1)$. Thus uniqueness fails. More precisely, there are infinitely many solutions if

$$
\int_0^\pi\phi(x)f(x)\,dx=c_1+\frac{c_2}{\pi-1},
$$

and none otherwise. This follows either from the scalar equation or by [integration by parts](../../../../../integration-by-parts.md) against $\phi$. It is the compatibility obstruction at [Dirichlet resonance for a point interaction](../../../../../dirichlet-resonance-for-a-point-interaction.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
