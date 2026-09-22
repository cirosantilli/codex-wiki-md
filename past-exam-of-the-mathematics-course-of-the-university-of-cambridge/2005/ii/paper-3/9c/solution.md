<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

The [Poisson bracket](../../../../../poisson-bracket.md) is $\{f,g\}=\sum_a(f_{q_a}g_{p_a}-f_{p_a}g_{q_a})$. For a function with no explicit time dependence, the chain rule and [Hamilton equations](../../../../../hamilton-s-equations.md) give

$$
\frac{df}{dt}=\sum_a(f_{q_a}\dot q_a+f_{p_a}\dot p_a)=\sum_a(f_{q_a}H_{p_a}-f_{p_a}H_{q_a})=\boxed{\{f,H\}}.
$$

With $L_b=\epsilon_{bcd}x_cp_d$, direct differentiation gives

$$
\boxed{\{p_a,L_b\}=-\epsilon_{bad}p_d=\epsilon_{abd}p_d,\qquad \{x_a,L_b\}=\epsilon_{abc}x_c.}
$$

Apply the product rule to $L_a=\epsilon_{acd}x_cp_d$ and substitute these two brackets. Contracting the epsilon symbols yields $\boxed{\{L_a,L_b\}=\epsilon_{abc}L_c}$. Equivalently, the two product terms are precisely the infinitesimal rotation of the vector $x\times p$ about the $b$ axis, with the same bracket convention as the position and momentum vectors.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
