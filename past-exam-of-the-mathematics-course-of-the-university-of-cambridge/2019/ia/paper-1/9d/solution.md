<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

The [Cauchy functional equation](../../../../../cauchy-s-functional-equation.md) first gives $g(0)=0$ and $g(-x)=-g(x)$. If $h\to0$, then continuity at the given point $z$ gives

$$
g(h)=g(z+h)-g(z)\longrightarrow0,
$$

so $g$ is continuous at zero. For every $x$,

$$
g(x+h)-g(x)=g(h)\longrightarrow0,
$$

so $g$ is continuous everywhere.

Put $c=g(1)$. Additivity gives $g(n)=nc$ for integers $n$ and then $g(m/n)=(m/n)c$ for [rational numbers](../../../../../rational-number.md). For any real $x$, choose rationals $q_j\to x$; continuity gives

$$
\boxed{g(x)=\lim_jg(q_j)=\lim_jcq_j=cx}.
$$

For the multiplicative equation, $h(0)=h(0)^2$. If $h(0)=0$, then $h(x)=h(x)h(0)=0$ for every $x$. Otherwise $h(0)=1$. In that case

$$
h(x)=h(x/2)^2\geq0,
$$

and $h(x)$ cannot vanish because $1=h(0)=h(x)h(-x)$. Hence $h$ is everywhere positive. The continuous function $g=\log h$ satisfies the [Cauchy functional equation](../../../../../cauchy-s-functional-equation.md), so $g(x)=cx$. Therefore the complete family is

$$
\boxed{h\equiv0\quad\text{or}\quad h(x)=e^{cx}\ \text{for some }c\in\mathbb R}.
$$

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
