<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Write $u_n=\mathbb P(X_n=0\mid X_0=0)$. The [Markov property](../../../../../markov-property.md), conditioning on the state at time $n$, gives

$$
u_{n+1}=\alpha u_n+(1-\beta)(1-u_n)=(\alpha+\beta-1)u_n+1-\beta,\qquad u_0=1.
$$

Put $r=\alpha+\beta-1$ and $\pi_0=(1-\beta)/(2-\alpha-\beta)$. Then $\pi_0=r\pi_0+1-\beta$, so subtraction yields $u_{n+1}-\pi_0=r(u_n-\pi_0)$. Iterating this [linear recurrence](../../../../../linear-recurrence-relation.md) gives

$$
\boxed{u_n=\frac{1-\beta+(1-\alpha)(\alpha+\beta-1)^n}{2-\alpha-\beta},\qquad n\geq0.}
$$

For $r=0$, read the $n=0$ expression using $r^0=1$, or state $u_0=1$ separately; for $n\geq1$, $u_n=\pi_0$. Since $|r|<1$, the result also shows [convergence in a metric space](../../../../../convergence-in-a-metric-space.md) to the [stationary distribution](../../../../../stationary-distribution.md) probability $\pi_0$.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
