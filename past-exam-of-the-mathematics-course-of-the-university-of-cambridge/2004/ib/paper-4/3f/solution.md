<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The map is [differentiable](../../../../../differentiable-function.md) at $u$ when there exists a [linear map](../../../../../linear-map.md) $A:\mathbb R^n\to\mathbb R^m$ such that

$$
\boxed{\lim_{h\to0}\frac{\|f(u+h)-f(u)-Ah\|}{\|h\|}=0.}
$$

The increments are taken sufficiently small to stay in the open domain; $A=Df(u)$ is the derivative. This is a joint approximation in all directions, not just the existence of coordinate partial derivatives.

At $(a,b)$ with $ab\ne0$, choose $\delta<\min(|a|,|b|)$. If $\|(h,k)\|<\delta$, neither coordinate changes sign, and

$$
g(a+h,b+k)-g(a,b)=\operatorname{sgn}(a)h+\operatorname{sgn}(b)k.
$$

Thus the remainder in the differentiability definition is identically zero throughout that neighborhood. Consequently

$$
\boxed{Dg(a,b)(h,k)=\operatorname{sgn}(a)h+\operatorname{sgn}(b)k,}
$$

which proves the requested differentiability directly.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
