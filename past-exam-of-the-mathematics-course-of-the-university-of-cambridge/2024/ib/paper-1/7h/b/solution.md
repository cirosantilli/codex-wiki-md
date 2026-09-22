<h1 id="7h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The dual from part (a) is

$$
\begin{aligned}
\text{maximise}\quad&7y+11z\\
\text{subject to}\quad
&y+z\leq3,\qquad y\leq2,\qquad z\leq2,\\
&y+2z\geq2,qquad y,z\geq0.
\end{aligned}
$$

The point $(y,z)=(1,2)$ is dual feasible and has value $29$. The primal point

$$
(x_1,x_2,x_3,x_4)=(7,0,4,0)
$$

is feasible and also has objective value

$$
3(7)+2(4)=29.
$$

By [weak duality](../../../../../../weak-duality.md), neither point can be improved, so

$$
\boxed{\min=29,\qquad(x_1,x_2,x_3,x_4)=(7,0,4,0)}.
$$

The strict dual inequalities for $x_2$ and $x_4$, together with [complementary slackness](../../../../../../complementary-slackness.md), force $x_2=x_4=0$ at any optimum; the two tight primal constraints then force $x_1=7$ and $x_3=4$. Thus the displayed minimizer is unique.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7H](../../7h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
