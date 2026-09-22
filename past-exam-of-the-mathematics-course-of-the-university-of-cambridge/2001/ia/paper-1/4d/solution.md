<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

Suppose $f$ is continuous on $[a,b]$, differentiable on $(a,b)$ and satisfies $f(a)=f(b)$, with $a<b$. Apply the [extreme value theorem](../../../../../extreme-value-theorem.md) to both $f$ and $-f$ to obtain a maximum and a minimum. If $f$ is constant, every interior derivative is zero. Otherwise some value differs from the common endpoint value, so either a maximum or a minimum occurs at an interior point $c$. At an interior maximum, difference quotients are nonpositive from the right and nonnegative from the left; since the [derivative](../../../../../derivative.md) exists, it must be zero. The minimum case is identical with the inequalities reversed. This proves **Rolle's theorem:** $\boxed{f'(c)=0}$ for some $c\in(a,b)$.

For the [mean value theorem](../../../../../mean-value-theorem.md), subtract the endpoint chord:

$$
g(t)=f(t)-f(a)-\frac{f(b)-f(a)}{b-a}(t-a).
$$

Then $g(a)=g(b)=0$, so [Rolle's theorem](../../../../../rolle-theorem.md) supplies $c\in(a,b)$ with $g'(c)=0$. Hence

$$
\boxed{f'(c)=\frac{f(b)-f(a)}{b-a}.}
$$

If $f'(t)>0$ everywhere, applying the [mean value theorem](../../../../../mean-value-theorem.md) to any $x<y$ gives $f(y)-f(x)=f'(c)(y-x)>0$. Thus $f$ is [strictly increasing](../../../../../strictly-increasing-function.md). **The converse is false:** $\boxed{f(t)=t^3}$ is [strictly increasing](../../../../../strictly-increasing-function.md) but $f'(0)=0$.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
