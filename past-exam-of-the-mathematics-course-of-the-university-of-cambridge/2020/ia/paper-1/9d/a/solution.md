<h1 id="9d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Rolle theorem](../../../../../../rolle-theorem.md) states that if $h$ is continuous on the closed interval between two distinct points, differentiable between them, and has equal endpoint values, then $h'$ vanishes at an interior point.

Let $P_N(t)=\sum_{j=0}^Nf^{(j)}(0)t^j/j!$ and, for $x\ne0$, put

$$
M=\frac{f(x)-P_N(x)}{x^{N+1}},
\qquad h(t)=f(t)-P_N(t)-Mt^{N+1}.
$$

Then $h(x)=0$ and $h^{(j)}(0)=0$ for $0\leq j\leq N$. Applying Rolle's theorem successively $N+1$ times gives a point $\xi=\theta x$, $0<\theta<1$, where $h^{(N+1)}(\xi)=0$. Hence

$$
M=\frac{f^{(N+1)}(\theta x)}{(N+1)!},
$$

which is the stated [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md).

If $f'=0$, the $N=0$ case gives $f(x)=f(0)+xf'(\theta x)=f(0)$. Thus $f$ is constant; equivalently this is the immediate corollary of the [mean value theorem](../../../../../../mean-value-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
