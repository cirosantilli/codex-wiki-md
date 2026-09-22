<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

[Differentiability](../../../../../differentiability.md) at $p$ means there is a [linear map](../../../../../linear-map.md) $A=Df|_p$ such that

$$
f(p+h)=f(p)+Ah+r(h),\qquad
\frac{\|r(h)\|}{\|h\|}\longrightarrow0\quad(h\to0).
$$

This is the [Fréchet derivative](../../../../../frechet-derivative.md) definition; the same linear approximation must work in every direction, not merely along coordinate axes.

The [chain rule](../../../../../chain-rule.md) says that if $f$ is [differentiable](../../../../../differentiable-function.md) at $p$ and $g$ is [differentiable](../../../../../differentiable-function.md) at $f(p)$, then $g\circ f$ is [differentiable](../../../../../differentiable-function.md) at $p$ and

$$
\boxed{D(g\circ f)|_p=Dg|_{f(p)}\circ Df|_p.}
$$

For its proof, put $A=Df|_p$, $B=Dg|_{f(p)}$, and $k=f(p+h)-f(p)=Ah+r(h)$. Since a [linear map](../../../../../linear-map.md) between these finite-dimensional normed spaces is bounded, $\|k\|=O(\|h\|)$. [Differentiability](../../../../../differentiability.md) of $g$ gives $g(f(p)+k)=g(f(p))+Bk+s(k)$ with $s(k)=o(\|k\|)$. Therefore

$$
g(f(p+h))-g(f(p))-BAh=Br(h)+s(k)=o(\|h\|).
$$

If $k=0$, take $s(0)=0$; otherwise $\|s(k)\|/\|h\|=(\|s(k)\|/\|k\|)(\|k\|/\|h\|)\to0$. This proves the required full linear approximation.

For the [Euclidean norm](../../../../../euclidean-norm.md), at every $x\ne0$ the ordinary one-coordinate differentiation gives

$$
\boxed{\frac{\partial\|x\|}{\partial x_i}=\frac{x_i}{\|x\|}.}
$$

At the origin its difference quotient in direction $e_i$ is $|t|/t$, whose right and left limits are $1$ and $-1$. Thus **none of its coordinate [partial derivatives](../../../../../partial-derivative.md) exists at the origin**.

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
