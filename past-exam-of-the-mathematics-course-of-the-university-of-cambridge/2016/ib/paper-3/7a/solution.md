<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

Away from $x=\xi$, a [Green function](../../../../../green-s-function.md) for this second-derivative operator is linear in $x$. The left [boundary condition](../../../../../boundary-condition.md) makes it $ax$ on $x<\xi$, and the right [Neumann boundary condition](../../../../../neumann-boundary-condition.md) makes it constant $b$ on $x>\xi$. Continuity gives $b=a\xi$. Integrating the distributional equation through the [Dirac delta function](../../../../../dirac-delta-function.md) gives the jump $G_x(\xi^+;\xi)-G_x(\xi^-;\xi)=1$, so $a=-1$. Therefore

$$
\boxed{G(x;\xi)=-\min(x,\xi)=
\begin{cases}-x,&x\leq\xi,\\-\xi,&x\geq\xi.\end{cases}}
$$

Apply the [Green function](../../../../../green-s-function.md) to the forcing:

$$
y(x)=\int_0^1G(x;\xi)\xi e^{-\xi}\,d\xi
=-\int_0^x\xi^2e^{-\xi}\,d\xi-x\int_x^1\xi e^{-\xi}\,d\xi.
$$

Evaluation yields

$$
\boxed{y(x)=(x+2)e^{-x}+\frac{2x}{e}-2.}
$$

Indeed $y'(x)=-(x+1)e^{-x}+2/e$, so $y''=xe^{-x}$, $y(0)=0$ and $y'(1)=0$. A difference of two solutions is linear with these homogeneous boundary conditions, hence zero; the [boundary value problem](../../../../../boundary-value-problem.md) has a unique solution.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
