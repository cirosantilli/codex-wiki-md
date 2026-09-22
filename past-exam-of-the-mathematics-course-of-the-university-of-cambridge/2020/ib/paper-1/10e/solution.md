<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

A function $f:\mathbb R^m\to\mathbb R^r$ is [differentiable](../../../../../differentiable-function.md) at $x$ if there is a linear map $L:\mathbb R^m\to\mathbb R^r$ such that

$$
f(x+h)=f(x)+Lh+o(\lVert h\rVert)
\quad\text{as }h\to0.
$$

The map $L$, which is unique, is the [derivative](../../../../../derivative.md) $f'(x)$.

Expanding in a matrix increment $H$ gives

$$
(A+H)^3=A^3+A^2H+AHA+HA^2+O(\lVert H\rVert^2).
$$

Therefore $p$ is differentiable everywhere and

$$
\boxed{p'(A)H=A^2H+AHA+HA^2-3H}.
$$

The [inverse function theorem](../../../../../inverse-function-theorem.md) states that if $f$ is [continuously differentiable](../../../../../continuously-differentiable-function.md) near $a$ and $f'(a)$ is invertible, then $f$ restricts to a bijection between neighbourhoods of $a$ and $f(a)$; its local inverse is continuously differentiable, with derivative

$$
(f^{-1})'(y)=\bigl[f'(f^{-1}(y))\bigr]^{-1}.
$$

In the normalized case $f(0)=0$ and $f'(0)=I$, continuity of $f'$ gives a closed ball $\overline B_r(0)$ on which

$$
\lVert I-f'(x)\rVert\le q<1.
$$

For small $y$, define $T_y(x)=x-f(x)+y$. The [mean value inequality](../../../../../mean-value-inequality.md) makes $T_y$ a [contraction mapping](../../../../../contraction-mapping.md) with constant $q$. If $\lVert y\rVert\le(1-q)r$, then

$$
\lVert T_y(x)\rVert\le q\lVert x\rVert+\lVert y\rVert\le r,
$$

so $T_y$ maps the ball into itself. The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) gives a unique [fixed point](../../../../../fixed-point.md) $x_y$, and the fixed-point equation is precisely $f(x_y)=y$. Moreover,

$$
\lVert x_y-x_z\rVert
\le q\lVert x_y-x_z\rVert+\lVert y-z\rVert,
$$

so $\lVert x_y-x_z\rVert\le\lVert y-z\rVert/(1-q)$. Thus $y\mapsto x_y$ is a continuous local inverse.

For the polynomial map in the question,

$$
p(2I)=I,
\qquad
p'(2I)H=(4+4+4-3)H=9H.
$$

The derivative is invertible, so the inverse function theorem supplies some $\epsilon>0$ and a continuously differentiable $q:D_\epsilon(I)\to\mathcal M_n$ such that

$$
\boxed{p\circ q=\operatorname{id}|_{D_\epsilon(I)}}.
$$

There can be no inverse on all of $\mathcal M_n$, because

$$
p(2I)=I=p(-I),
$$

so $p$ is not [injective](../../../../../injective-function.md).

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
