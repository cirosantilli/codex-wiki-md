<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The homogeneous [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $r^2-2r+2=0$, with roots $1\pm i$. Choose the endpoint-adapted homogeneous solutions

$$
u(x)=e^x\sin x,\qquad v(x)=e^x\cos x,
$$

so that $u(0)=0$ and $v(\pi/2)=0$. Their [Wronskian](../../../../../wronskian.md) is

$$
W(x)=u(x)v'(x)-u'(x)v(x)=-e^{2x},
$$

which never vanishes. A continuous [Green function](../../../../../green-s-function-split.md) with the required endpoints has the form $C(\xi)u(x_<)v(x_>)$, where $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$. Its [derivative](../../../../../derivative.md) jump is $C(\xi)W(\xi)$. Because the leading coefficient is one, part (b) requires this to equal one. Therefore

$$
\boxed{G(x;\xi)=-e^{x-\xi}\sin x_<\cos x_>.}
$$

In particular, the branches are $-e^{x-\xi}\sin x\cos\xi$ for $x\leq\xi$ and $-e^{x-\xi}\sin\xi\cos x$ for $x\geq\xi$. This is the [Dirichlet Green function for a conjugated harmonic oscillator](../../../../../dirichlet-green-function-for-a-conjugated-harmonic-oscillator.md) with interval length $\pi/2$, drift parameter one and oscillator wave number one.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
