<h1 id="8d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand the second stage by the [Taylor theorem](../../../../../../taylor-theorem.md), writing $f=f(t_n,y_n)$ and $D_yf$ for the derivative in the state variable:

$$
k_2=f+\frac h2\bigl(f_t+(D_yf)f\bigr)+O(h^2).
$$

The update therefore agrees with the exact solution's [Taylor series](../../../../../../taylor-series.md):

$$
y_{n+1}=y_n+hf+\frac{h^2}{2}\bigl(f_t+(D_yf)f\bigr)+O(h^3).
$$

Thus the one-step [local truncation error](../../../../../../local-truncation-error.md) is $O(h^3)$, and the method has order at least two under the usual smoothness and [Lipschitz continuity](../../../../../../lipschitz-continuity.md) assumptions.

For $f=\lambda y$, the two-stage [Runge-Kutta method](../../../../../../runge-kutta-method.md) gives

$$
\boxed{R(z)=1+z+\frac{z^2}{2}.}
$$

On the real axis, $R(z)=\tfrac12(z+1)^2+\tfrac12\geq\tfrac12$, so $|R(z)|\leq1$ is equivalent to $(z+1)^2\leq1$. Hence

$$
\boxed{\mathcal S\cap\mathbb R=[-2,0].}
$$

The decay convention gives $(-2,0)$. Since negative real values such as $z=-3$ lie outside the [linear stability domain](../../../../../../linear-stability-domain.md), the method is **not A-stable**. Its order is exactly two, since $R(z)$ lacks the cubic term of $e^z$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8D](../../8d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
