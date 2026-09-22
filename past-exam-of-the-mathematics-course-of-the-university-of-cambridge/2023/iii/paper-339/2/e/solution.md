<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $w_k=(x_k,z_k)$ and $w_{k+1}=(x_{k+1},z_{k+1})$. Expanding

$$
M w_{k+1}+F(w_{k+1})=Mw_k
$$

gives

$$
\begin{aligned}
\alpha x_{k+1}+A^Tz_{k+1}
+\nabla f(x_{k+1})-A^Tz_{k+1}
&=\alpha x_k+A^Tz_k,\\
Ax_{k+1}+\beta z_{k+1}
+Ax_{k+1}-b
&=Ax_k+\beta z_k.
\end{aligned}
$$

The off-diagonal terms in the first equation cancel. By the optimality condition for the [proximal operator](../../../../../../proximal-operator.md),

$$
\boxed{
x_{k+1}
=\operatorname{prox}_{\alpha^{-1}f}
\left(x_k+\alpha^{-1}A^Tz_k\right).}
$$

The second equation then becomes the explicit linear update

$$
\boxed{
z_{k+1}
=z_k+\beta^{-1}\bigl(Ax_k-2Ax_{k+1}+b\bigr).}
$$

**Thus each step of this [preconditioned proximal point algorithm](../../../../../../preconditioned-proximal-point-algorithm.md) uses only one evaluation of the [proximal operator](../../../../../../proximal-operator.md) of $\alpha^{-1}f$, together with applications of the [linear map](../../../../../../linear-map.md) $A$ and its [transpose](../../../../../../transpose.md) $A^T$.**

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
