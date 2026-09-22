<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $h\in(0,1)$, $X=\alpha h+O(\alpha^3)$ and $Y=\alpha(1-h)+O(\alpha^3)$. The factored [dispersion relation](../../../../../../dispersion-relation.md) therefore gives

$$
\lim_{\alpha\to0}c^2=2h-1,\qquad
\lim_{\alpha\to\infty}c^2=1,
$$

where the latter follows from $X,Y\to1$ and $c^2\sim(1-1/(2\alpha h))^2$. A real negative $c^2$ yields a growing branch $c=i\sqrt{-c^2}$ for positive $k$. Thus $h<1/2$ gives instability at sufficiently small nonzero wavenumber.

For the converse, monotonicity toward the limiting value one would suffice, as permitted in the question. In fact a direct sign argument avoids this extra assumption. With $q=\alpha h>0$, $X=\tanh q<q$, so $J-XY=qX+(q-X)Y>0$. If $h\ge1/2$, then $q\ge d=\alpha(1-h)$ and $Y=\tanh d<d\le q$. Hence $H-Y=q(1+XY)-Y>0$, so $c^2>0$ for every $\alpha>0$. We obtain the exact [instability threshold for a bounded piecewise-linear shear layer](../../../../../../instability-threshold-for-a-bounded-piecewise-linear-shear-layer.md):

$$
\boxed{0<\zeta_L<\frac12\quad\text{is the condition for exponential linear instability}.}
$$

At $\zeta_L=1/2$ the long-wave limiting value is zero, but every finite positive wavenumber has $c^2>0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
