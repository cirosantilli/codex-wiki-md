<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

When $M=G$ is a [group](../../../../../../group-split.md), evaluation at its identity gives a bijection from the previous equivariant-map set to all functions $X\to Y$. For an arbitrary function $f$, the inverse construction is

$$
e_f(g,x)=f(xg^{-1})g.
$$

Indeed,

$$
e_f(gk,xk)=f(xk(gk)^{-1})gk=f(xg^{-1})gk=e_f(g,x)k,
$$

so $e_f$ is an [equivariant map](../../../../../../equivariant-map.md). Conversely, if $e$ is equivariant, $(g,x)=(1,xg^{-1})g$ implies $e(g,x)=e(1,xg^{-1})g$, so $e=e_f$ for $f(x)=e(1,x)$.

Transport the right action from part (a) through this bijection. At $x$ its value is

$$
(ek)(1,x)=e(k,x)=f(xk^{-1})k.
$$

Thus the [exponential of right group actions](../../../../../../exponential-of-right-group-actions.md) is

$$
\boxed{Y^X=\operatorname{Set}(X,Y),\qquad (fk)(x)=f(xk^{-1})k.}
$$

For clarity, the right-action law holds even in a nonabelian [group](../../../../../../group-split.md):

$$
((fk)l)(x)=f(xl^{-1}k^{-1})kl=f(x(kl)^{-1})kl=(f(kl))(x).
$$

Evaluation is equivariant because $(fk)(xk)=f(x)k$. The underlying functions need not be equivariant; the fixed points of this exponential action are exactly the equivariant functions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
