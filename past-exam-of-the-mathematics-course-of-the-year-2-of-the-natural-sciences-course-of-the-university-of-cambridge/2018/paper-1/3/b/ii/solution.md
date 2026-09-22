<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The reduced forcing is $f(\xi)=\xi\,\mathbf1_{[1,\infty)}(\xi)$. Its exponential-weighted integrals converge, even though the resulting reduced function is not bounded. For $0\leq x<1$, the [Green's function](../../../../../../green-s-function-split.md) formula gives

$$
y(x)=-\sinh x\int_1^\infty\xi e^{-\xi}\,d\xi=-\frac2e\sinh x.
$$

For $x\geq1$ it gives

$$
y(x)=-e^{-x}\int_1^x\xi\sinh\xi\,d\xi-\sinh x\int_x^\infty\xi e^{-\xi}\,d\xi.
$$

Use $\int\xi\sinh\xi\,d\xi=\xi\cosh\xi-\sinh\xi$ and $\int_x^\infty\xi e^{-\xi}\,d\xi=(x+1)e^{-x}$ to simplify this to $y(x)=-x+e^{-x-1}$. Dividing by $x$ yields

$$
\boxed{u(x)=\begin{cases}
\displaystyle-\frac2e\frac{\sinh x}{x},&0<x<1,\\[5pt]
\displaystyle-1+\frac{e^{-x}}{ex},&x\geq1,
\end{cases}\qquad u(0)=-\frac2e,\quad A=\frac1e}.
$$

Thus $a(x)=-(2/e)\sinh x/x$ with its continuous value at zero. At $x=1$, both pieces give $u=-1+e^{-2}$ and $u'=-2e^{-2}$, so neither a [Dirac delta distribution](../../../../../../dirac-delta-function.md) nor its [derivative](../../../../../../derivative.md) is introduced at the forcing jump. The solution is bounded at both ends, with $u\to-1$ at infinity. Its reduced function $y=xu\sim-x$ confirms the growth qualification in part (i).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
