<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

Introduce nonnegative [slack variables](../../../../../slack-variable.md) $s_1,s_2,s_3$ and start the [simplex algorithm](../../../../../simplex-algorithm.md) at $x=y=z=0$, with slacks $9,8,2$. The objective's largest positive entering coefficient belongs to $y$. Its ratio test is $9/3=3$, $8/2=4$, $2/1=2$, so $s_3$ leaves and $y$ enters.

Solve that pivot row for $y$ and substitute into the other rows and the objective $v$:

$$
\begin{aligned}
y&=2-2x-3z-s_3,\\
s_1&=3-2x-z+3s_3,\\
s_2&=4-x+2z+2s_3,\\
v&=10-7x-15z-5s_3.
\end{aligned}
$$

This is a feasible [simplex dictionary](../../../../../simplex-dictionary.md) at nonbasic variables $x=z=s_3=0$. All their objective coefficients are negative, so no feasible increase can improve the objective. Thus

$$
\boxed{(x,y,z)=(0,2,0),\qquad v_{\max}=10.}
$$

The negative reduced coefficients also prove uniqueness of this optimum.

The [dual linear program](../../../../../dual-linear-program.md), with nonnegative variables $u_1,u_2,u_3$, is

$$
\begin{gathered}
\text{minimize }9u_1+8u_2+2u_3,\\
8u_1+5u_2+2u_3\ge3,\quad3u_1+2u_2+u_3\ge5,\quad10u_1+4u_2+3u_3\ge0.
\end{gathered}
$$

The feasible choice $\boxed{(u_1,u_2,u_3)=(0,0,5)}$ has objective $10$. [Weak duality](../../../../../weak-duality.md) proves that it and the primal point are optimal. [Complementary slackness](../../../../../complementary-slackness.md) also forces $u_1=u_2=0$ because the first two primal slacks are positive, and then the positive $y$ forces $u_3=5$.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
