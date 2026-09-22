<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

The [mean value theorem](../../../../../mean-value-theorem.md) states that a real-valued function continuous on $[a,b]$ and differentiable on $(a,b)$, with $a<b$, has a point $\xi\in(a,b)$ such that

$$
\boxed{f'(\xi)=\frac{f(b)-f(a)}{b-a}.}
$$

For the proof, subtract the secant line and put $h(t)=f(t)-f(a)-(t-a)[f(b)-f(a)]/(b-a)$. Then $h(a)=h(b)=0$. If $h$ is identically zero, every interior point works. Otherwise it has a positive maximum or a negative minimum. The [extreme value theorem](../../../../../extreme-value-theorem.md) supplies that extremum, and its nonzero value makes its location interior. At an interior differentiable extremum, the difference quotients on the two sides have opposite weak signs, so their common [limit](../../../../../limit-of-a-function.md) is zero. Hence $h'(\xi)=0$, proving the formula. This also gives the [Rolle theorem](../../../../../rolle-theorem.md) argument rather than merely citing it.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
