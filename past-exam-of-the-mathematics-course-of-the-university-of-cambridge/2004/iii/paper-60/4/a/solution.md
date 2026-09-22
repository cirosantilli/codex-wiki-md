<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After one iteration $y_n\in\{1,-1\}$, so work on that invariant sign sheet. For $x_n\ne0$,

$$
\begin{aligned}
z_{n+1}&=-x_{n+1}y_{n+1}
=\mu-A\operatorname{sgn}(y_n)\operatorname{sgn}(x_n)|x_n|^\delta\\
&=\boxed{\mu+A\operatorname{sgn}(z_n)|z_n|^\delta},
\end{aligned}
$$

since $z_n=-x_ny_n$ and $|y_n|=1$. This is the [signed gluing-map reduction](../../../../../../signed-gluing-map-reduction.md). If an arbitrary initial value of $y$ is admitted, the formula applies after that first iterate, not before it. The point $z=0$ represents a [separatrix](../../../../../../separatrix.md) at which the original flow return is singular, even though the scalar map can be extended continuously there.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
