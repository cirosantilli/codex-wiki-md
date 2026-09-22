<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Away from $x=\xi$, the homogeneous equation has solutions $e^x,e^{-x}$. A basis adapted to the two [boundary conditions](../../../../../boundary-condition.md) is $u(x)=\sinh x$ at the origin and $v(x)=e^{-x}$ at infinity. Their [Wronskian](../../../../../wronskian.md) is $uv'-u'v=-1$. The [Green function](../../../../../green-s-function-split.md) must be continuous at $\xi$, while [integration](../../../../../integral-split.md) of $-G_{xx}+G=\delta(x-\xi)$ across the source gives

$$
G_x(\xi+,\xi)-G_x(\xi-,\xi)=-1.
$$

These conditions give the [Dirichlet half-line Green function for minus d2 plus 1](../../../../../dirichlet-half-line-green-function-for-minus-d2-plus-1.md):

$$
\boxed{G(x,\xi)=\sinh(x_<)e^{-x_>}=\frac12\left(e^{-|x-\xi|}-e^{-(x+\xi)}\right),}
$$

where $x_<=\min(x,\xi)$ and $x_>=\max(x,\xi)$. The second term is the image that enforces $G(0,\xi)=0$; both terms decay as $x\to\infty$.

For the finite forcing interval, $y(x)=\int_0^\mu G(x,\xi)\,d\xi$. When $x\leq\mu$, split the [integral](../../../../../integral-split.md) at $\xi=x$:

$$
y(x)=e^{-x}\int_0^x\sinh\xi\,d\xi+\sinh x\int_x^\mu e^{-\xi}\,d\xi=1-e^{-x}-e^{-\mu}\sinh x.
$$

When $x\geq\mu$, the entire source interval lies to the left, giving the [Dirichlet half-line response to uniform interval forcing](../../../../../dirichlet-half-line-response-to-uniform-interval-forcing.md)

$$
\boxed{y(x)=\begin{cases}1-e^{-x}-e^{-\mu}\sinh x,&0\leq x\leq\mu,\\(\cosh\mu-1)e^{-x},&x\geq\mu.\end{cases}}
$$

This solution is unique: a homogeneous difference satisfying the origin condition is proportional to $\sinh x$, which cannot decay at infinity unless its coefficient is zero.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
