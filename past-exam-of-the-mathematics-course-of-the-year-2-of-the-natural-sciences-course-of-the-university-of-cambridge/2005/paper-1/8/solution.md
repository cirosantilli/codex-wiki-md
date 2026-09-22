<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Take $x\geq0$ and a source position $\xi>0$. Before the source, the zero initial data require $G=0$. After it, set $G=e^{-2(x-\xi)}h(x-\xi)$; the homogeneous equation becomes $h''+a^2h=0$. Continuity of $G$ and a unit jump in $G_x$ at $x=\xi$ give $h(0)=0$, $h'(0)=1$. Thus the [causal Green function of a damped oscillator](../../../../causal-green-function-of-a-damped-oscillator.md) is

$$
\boxed{G(x,\xi)=H(x-\xi)e^{-2(x-\xi)}\frac{\sin[a(x-\xi)]}{a}.}
$$

Here $H$ is the [Heaviside step function](../../../../heaviside-step-function.md). For $a=0$, take the continuous limit $\sin(as)/a\to s$, giving $G=H(x-\xi)(x-\xi)e^{-2(x-\xi)}$. The formula is also unchanged when a nonzero $a$ changes sign. Its continuity removes a delta derivative, and its unit first-derivative jump supplies the required [Dirac delta function](../../../../dirac-delta-function.md).

For the forced equation use $a=2$. The zero-initial-data [Green function](../../../../green-s-function-split.md) representation is

$$
y(x)=\frac12\int_0^xe^{-2(x-\xi)}\sin[2(x-\xi)]\sin2\xi\,d\xi.
$$

The sine-product identity reduces this to elementary exponential-trigonometric integrals. Evaluating gives

$$
\boxed{y(x)=\frac{\sin2x-2\cos2x+e^{-2x}(2\cos2x+\sin2x)}{20}.}
$$

For an independent check, the steady particular part is $\sin2x/20-\cos2x/10$, while the decaying homogeneous part has coefficients $1/10$ and $1/20$ that impose $y(0)=y'(0)=0$.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
