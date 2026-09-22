<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

For the [additive function](../../../../../additive-function.md), setting both arguments to zero gives $f(0)=0$, and then $f(-x)=-f(x)$. Continuity at the given point $x_0$ implies

$$
f(h)=f(x_0+h)-f(x_0)\longrightarrow0\qquad(h\to0).
$$

For any real $x$, $f(x+h)-f(x)=f(h)$, so $f$ is continuous at every point. This proves the continuity part of [additive function continuous at one point is linear](../../../../../additive-function-continuous-at-one-point-is-linear.md).

Let $c=f(1)$. Repeated addition and negation give $f(m)=mc$ for every integer $m$. For integers $p$ and positive $q$,

$$
qf(p/q)=f(p)=pc,
$$

so $f(r)=cr$ for every [rational number](../../../../../rational-number.md) $r$. Given any real $x$, choose rational $r_n\to x$. Continuity and [density of the rational numbers](../../../../../density-of-the-rational-numbers.md) give

$$
\boxed{f(x)=\lim_n f(r_n)=\lim_n cr_n=cx.}
$$

Conversely each real multiple of $x$ satisfies the [Cauchy functional equation](../../../../../cauchy-s-functional-equation.md).

For the multiplicative equation, assume first that $g$ is not identically zero and choose $x_1$ with $g(x_1)\ne0$. Then $g(x_1)=g(x_1)g(0)$ forces $g(0)=1$. Next

$$
g(x)g(-x)=1
$$

makes every value nonzero, and

$$
g(x)=g(x/2)^2>0
$$

makes every value positive. Thus $h(x)=\log g(x)$ is a continuous real [additive function](../../../../../additive-function.md), since $h(x+y)=h(x)+h(y)$. The proved classification gives $h(x)=kx$ for a real constant $k$. This solves the [continuous exponential functional equation](../../../../../continuous-exponential-functional-equation.md):

$$
\boxed{g(x)\equiv0\quad\text{or}\quad g(x)=e^{kx}\ (k\in\mathbb R).}
$$

Both types satisfy the equation and continuity, and every nonzero solution is everywhere strictly positive.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
