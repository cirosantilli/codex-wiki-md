<h1 id="1/3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Because $f'$ is a decreasing bijection, its inverse $h$ exists and is continuous. For any $y$, choose $s=h((x-y)/t)$ in the preceding inequality. The line from $(0,y)$ then reaches $(t,x)$, giving $U(t,x)\ge U(0,y)+t g((x-y)/t)$.

Now let $x_0=X_t^{-1}(x)$ and $s=u_0(x_0)$. On this [characteristic curve](../../../../../../../characteristic-curve.md), $u=s$, so the tangent-line inequality is an equality throughout. This proves attainment and

$$
\boxed{U(t,x)=\max_{y\in\mathbb R}\left\{U(0,y)+t g\left(\frac{x-y}{t}\right)\right\},\qquad u(t,x)=h\left(\frac{x-x_0}{t}\right).}
$$

In fact the maximizing foot is unique. The [concave Legendre dual](../../../../../../../concave-legendre-dual.md) can be written $g(z)=\inf_s(zs-f(s))$ and satisfies $g'(z)=h(z)$: compare the minimizing values at $z$ and $z+\varepsilon$ and use continuity of $h$. This avoids assuming differentiability of $h$, which strict [concavity](../../../../../../../concave-function.md) by itself does not guarantee. Differentiating the maximizing expression with respect to $y$ gives $u_0(y)-h((x-y)/t)=0$, hence $X_t(y)=x$ and $y=x_0$. The [maximum representation for a concave conservation law](../../../../../../../maximum-representation-for-a-concave-conservation-law.md) therefore reproduces the [characteristic solution of a scalar conservation law](../../../../../../../characteristic-solution-of-a-scalar-conservation-law.md) throughout the smooth lifespan.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [1](../../../1.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
