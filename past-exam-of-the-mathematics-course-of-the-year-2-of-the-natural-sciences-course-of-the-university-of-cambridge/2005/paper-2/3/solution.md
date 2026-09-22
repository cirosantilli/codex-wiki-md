<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Compute the complex derivative along real increments to get $f'=u_x+iv_x$, and along imaginary increments to get $f'=v_y-iu_y$. Equality gives the [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md), $\boxed{u_x=v_y,\quad u_y=-v_x}$.

For the specified real part, observe that $iz e^{-z}=e^{-x}[(x\sin y-y\cos y)+i(x\cos y+y\sin y)]$. Thus the most general [holomorphic function](../../../../holomorphic-function-split.md) with this real part on the connected plane is

$$
\boxed{f(z)=iz e^{-z}+iC,\quad C\in\mathbb R.}
$$

The difference of two such holomorphic functions has zero real part, so the [Cauchy-Riemann equations](../../../../cauchy-riemann-equations.md) make its imaginary part constant.

Next, $\cosh z=\cosh x\cos y+i\sinh x\sin y$. Its real and imaginary parts satisfy $u_x=\sinh x\cos y=v_y$ and $u_y=-\cosh x\sin y=-v_x$. Their partial derivatives are continuous everywhere, proving that the complex [hyperbolic cosine](../../../../hyperbolic-cosine.md) is entire.

For the [Laurent series](../../../../laurent-series.md), set $h=z-1$. Since $z^2-1=h(2+h)$,

$$
\frac{\cosh z}{z^2-1}=\frac{\cosh1+h\sinh1+O(h^2)}{2h}\left(1-\frac h2+O(h^2)\right).
$$

The [regular part at a simple pole](../../../../regular-part-at-a-simple-pole.md) therefore gives

$$
\boxed{a_{-1}=\frac{\cosh1}{2},\qquad a_0=\frac{\sinh1}{2}-\frac{\cosh1}{4}.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 2](../../paper-2-split.md)
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
