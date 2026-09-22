<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

If $F=b\circ a$ with $a:\mathbb R^2\to\mathbb R$ and $b:\mathbb R\to\mathbb R^2$, the [chain rule](../../../../../chain-rule.md) gives $DF=Db\,Da$, the product of a two-by-one and a one-by-two [matrix](../../../../../matrix.md). Its [rank](../../../../../rank-one-quadratic-form.md) is at most one, so **its [Jacobian determinant](../../../../../jacobian-determinant.md) is identically zero**.

Conversely, [continuity](../../../../../continuous-function.md) and $f_y(0,0)\ne0$ give a neighborhood $U$ on which $f_y$ stays nonzero. The identity $f_xg_y-f_yg_x=0$ then implies $g_x=f_xg_y/f_y$. Therefore the smooth function $e=g_y/f_y$ satisfies

$$
\boxed{\nabla g=e\nabla f\quad\hbox{on }U.}
$$

For a graph curve $c(t)=(t,\alpha(t))$ with $F\circ c$ constant, the first component must have derivative zero. Thus the necessary equation is

$$
\boxed{\alpha'(t)=-\frac{f_x(t,\alpha(t))}{f_y(t,\alpha(t))}.}
$$

It is also sufficient: it makes $d(f\circ c)/dt=0$, and then $d(g\circ c)/dt=e\,d(f\circ c)/dt=0$.

To justify the existence through every nearby point, choose a closed rectangle about the origin inside $U$. The right-hand side $h(t,y)=-f_x/f_y$ is smooth there, hence bounded and locally Lipschitz in $y$. The [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) supplies a unique local solution through every initial point $(t_0,y_0)$ in a smaller open rectangle $V$. The boundedness of $h$ and a positive distance from the smaller rectangle to the outer boundary permit a common sufficiently short time interval about each $t_0$ on which the solution stays in $U$. Each point of $V$ therefore lies on one of these graph curves, and the preceding chain-rule calculation proves that $F$ is constant along it. This proves [rank-one level curves from a characteristic differential equation](../../../../../rank-one-level-curves-from-a-characteristic-differential-equation.md) using local ODE existence. The curves are local in their time parameter; no unjustified global existence for all real $t$ is required.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
