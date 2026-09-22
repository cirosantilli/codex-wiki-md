<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The homogeneous [Cauchy-Euler equation](../../../../cauchy-euler-equation.md) has solutions $x$ and $x^{-1}$. Choose $y_L=x$, which vanishes at zero, and $y_R=x-x^{-1}$, which vanishes at one. Their [Wronskian](../../../../wronskian.md) is $W(s)=y_L(s)y_R'(s)-y_L'(s)y_R(s)=2/s$. For a [Green function](../../../../green-s-function-split.md) integrated against the unweighted measure $ds$, continuity at $x=s$ and the jump condition $s^2[G_x]_{s^-}^{s^+}=1$ give

$$
\boxed{G(x,s)=\begin{cases}
\dfrac{x}{2}(1-s^{-2}),&0<x\leq s<1,\\[4pt]
\dfrac12(x-x^{-1}),&0<s\leq x<1.
\end{cases}}
$$

It satisfies $L_xG=\delta(x-s)$ for $L=x^2\partial_x^2+x\partial_x-1$. Therefore the candidate solution is

$$
\boxed{u(x)=\frac{x-x^{-1}}2\int_0^xf(s)ds+\frac x2\int_x^1(1-s^{-2})f(s)ds.}
$$

The leading coefficient vanishes at zero, so the endpoint condition needs care. If $f$ extends continuously to $[0,1]$, this expression has limit $-f(0)$ as $x\downarrow0$. Indeed $x^{-1}\int_0^xf(s)ds\to f(0)$ and $x\int_x^1f(s)s^{-2}ds\to f(0)$, while the remaining terms vanish. Thus the continuous zero-endpoint problem in this class requires **$f(0)=0$**. With that compatibility condition the formula gives both boundary values and is unique: a difference of two bounded solutions is $Ax+B/x$, whose two endpoint conditions force both constants to vanish. For incompatible forcing such as $f\equiv1$, the bounded solution with $u(1)=0$ is $x-1$, which cannot also vanish at zero. Pointwise vanishing of $G(x,s)$ for fixed $s$ does not justify interchanging the singular endpoint limit with its integral. This issue is treated in [Green kernel and endpoint compatibility for a singular Euler equation](../../../../green-kernel-and-endpoint-compatibility-for-a-singular-euler-equation.md).

For the supplied compatible forcing $f(s)=s$, the integrals are $x^2/2$ and $(1-x^2)/2+\log x$. Their polynomial pieces cancel, giving

$$
\boxed{u(x)=\frac{x\log x}{2}.}
$$

Direct differentiation gives $Lu=x$, and $x\log x\to0$ at zero. Its derivative diverges there, which is allowed because the boundary condition requires the value, not a finite derivative.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
