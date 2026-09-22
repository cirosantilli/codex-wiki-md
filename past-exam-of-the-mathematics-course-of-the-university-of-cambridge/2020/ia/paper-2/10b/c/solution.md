<h1 id="10b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose $u_1,u_2$ are solutions and put $w=u_1-u_2$. Then $\Delta w=0$ and $w$ satisfies the homogeneous [Robin boundary condition](../../../../../../robin-boundary-condition.md)

$$
(1-\lambda)w+\lambda\frac{\partial w}{\partial n}=0.
$$

For $0<\lambda<1$, [Green's first identity](../../../../../../green-s-first-identity.md) gives

$$
\int_V|\nabla w|^2\,dV
=\int_Sw\frac{\partial w}{\partial n}\,dS
=-\frac{1-\lambda}{\lambda}\int_Sw^2\,dS\leq0.
$$

The left side is nonnegative, so both sides vanish and $w=0$. For $\lambda=0$, the [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) $w=0$ on $S$ and the same identity again imply $w=0$. The solution is therefore unique for every $0\leq\lambda<1$.

For a regular spherically symmetric solution, the [Laplacian](../../../../../../laplacian.md) equation is

$$
\frac1{r^2}\frac d{dr}\left(r^2u'\right)=6.
$$

Regularity at the origin gives $u'=2r$, hence $u=r^2+C$. Applying the boundary condition at $r=b$ yields

$$
\boxed{u(r)=r^2-b^2-\frac{2\lambda b}{1-\lambda}},
\qquad 0\leq\lambda<1.
$$

At $\lambda=1$ the [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) would require $u'(b)=2b=0$, which is impossible for $b>0$. Equivalently, its compatibility condition would require $\int_V6\,dV=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10B](../../10b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
