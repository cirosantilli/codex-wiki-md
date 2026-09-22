<h1 id="32c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $V_1=\partial_x$, one has $\xi=1$, $\eta=0$, and hence $D_x\xi=0$. The recursion from part a gives $\eta_j=0$ for every $j$.

For $V_2=x\partial_x$, one has $D_x\xi=1$. Starting from $\eta_0=0$, induction gives

$$
\eta_j=-ju_j.
$$

For $V_3=x^2\partial_x$, one has $D_x\xi=2x$. The first coefficients are $\eta_1=-2xu_1$ and $\eta_2=-2u_1-4xu_2$, and induction gives

$$
\eta_j=-2jx u_j-j(j-1)u_{j-1}.
$$

Thus the three [prolongations of the projective vector fields on the line](../../../../../../prolongations-of-the-projective-vector-fields-on-the-line.md) are

$$
\boxed{
\begin{aligned}
\operatorname{pr}^{(n)}V_1
&=\partial_x,\\
\operatorname{pr}^{(n)}V_2
&=x\partial_x-\sum_{j=1}^n j u_j\partial_{u_j},\\
\operatorname{pr}^{(n)}V_3
&=x^2\partial_x-\sum_{j=1}^n
\bigl(2jx u_j+j(j-1)u_{j-1}\bigr)\partial_{u_j}.
\end{aligned}}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32C](../../32c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
