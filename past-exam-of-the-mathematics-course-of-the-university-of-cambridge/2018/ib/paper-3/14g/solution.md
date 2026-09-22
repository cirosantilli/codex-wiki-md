<h1 id="14g/solution">Solution</h1>

↑ **Parent:** [14G](../14g.md)

For a coordinate curve $v=v_0$, the length between $u_1$ and $u_2$ is

$$
L_v(u_1,u_2)=\int_{u_1}^{u_2}\sqrt{E(u,v_0)}\,du,
$$

where $E$ is a coefficient of the [first fundamental form](../../../../../first-fundamental-form.md). Thus $\partial E/\partial v=0$ makes the two $u$-directed sides of every coordinate rectangle equally long. Similarly,

$$
L_u(v_1,v_2)=\int_{v_1}^{v_2}\sqrt{G(u_0,v)}\,dv,
$$

so $\partial G/\partial u=0$ makes the two $v$-directed sides equally long.

Conversely, suppose every pair of opposite sides has equal length. Fix $v_0,v_1$. Equality of the first pair for every interval $[u_1,u_2]$ gives

$$
\int_{u_1}^{u_2}\left(\sqrt{E(u,v_0)}-\sqrt{E(u,v_1)}\right)du=0.
$$

The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) implies that the continuous integrand vanishes, so $E$ is independent of $v$. The same argument shows that $G$ is independent of $u$. Hence the stated equal-length property is equivalent to **$E_v=G_u=0$**.

## ↑ Ancestors (10)

1. [14G](../14g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
