<h1 id="13a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [diffusion approximation of a birth-death process](../../../../../../diffusion-approximation-of-a-birth-death-process.md) uses the first two jump moments. For these unit upward and downward jumps they give

$$
\boxed{
u(x)=\alpha+\beta x-\gamma x(x-1),\qquad
D(x)=\frac12\{\alpha+\beta x+\gamma x(x-1)\}.}
$$

The factor $1/2$ in $D$ is required because the equation is written with $+\partial_x^2(DP)$, rather than $\tfrac12\partial_x^2(BP)$.

Assuming the boundary terms vanish, integration by parts gives

$$
\begin{aligned}
\frac d{dt}\langle x\rangle
&=\int x\left[-\frac{\partial(uP)}{\partial x}
+\frac{\partial^2(DP)}{\partial x^2}\right]dx\\
&=\int u(x)P(x,t)\,dx=\langle u(x)\rangle.
\end{aligned}
$$

Consequently

$$
\boxed{
\frac d{dt}\langle x\rangle
=\alpha+\beta\langle x\rangle
-\gamma\langle x(x-1)\rangle,}
$$

which is precisely the discrete first-moment equation in part (b).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [13A](../../13a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
