<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce nonnegative [slack variables](../../../../../../slack-variable.md) $r_1,\ldots,r_4$ for the four dual inequalities. The initial [simplex dictionary](../../../../../../simplex-dictionary.md) is

$$
\begin{aligned}
r_1&=2-\lambda_1+2\lambda_3,&r_2&=4-2\lambda_1-2\lambda_2,\\
r_3&=3+\lambda_1-\lambda_2-3\lambda_3,&r_4&=1+3\lambda_2-\lambda_3,\\
z&=3\lambda_1+4\lambda_2+\lambda_3.
\end{aligned}
$$

At the origin all four basic slacks are positive. Enter $\lambda_2$: the [simplex ratio test](../../../../../../simplex-ratio-test.md) compares bounds $2$ from $r_2$ and $3$ from $r_3$, so $r_2$ leaves at $\lambda_2=2$. Entering $\lambda_1$ initially would tie two limiting bounds and produce [degeneracy in linear programming](../../../../../../degeneracy-in-linear-programming.md); the chosen pivot avoids this. The new [simplex dictionary](../../../../../../simplex-dictionary.md) is

$$
\begin{aligned}
\lambda_2&=2-\lambda_1-\tfrac12r_2,\\
r_1&=2-\lambda_1+2\lambda_3,\\
r_3&=1+2\lambda_1+\tfrac12r_2-3\lambda_3,\\
r_4&=7-3\lambda_1-\tfrac32r_2-\lambda_3,\\
z&=8-\lambda_1-2r_2+\lambda_3.
\end{aligned}
$$

Only $\lambda_3$ has positive objective coefficient. Enter it; the limiting bound is $1/3$ from $r_3$, rather than $7$ from $r_4$. Thus $r_3$ leaves, giving

$$
\begin{aligned}
\lambda_2&=2-\lambda_1-\tfrac12r_2,\\
\lambda_3&=\tfrac13+\tfrac23\lambda_1+\tfrac16r_2-\tfrac13r_3,\\
r_1&=\tfrac83+\tfrac13\lambda_1+\tfrac13r_2-\tfrac23r_3,\\
r_4&=\tfrac{20}3-\tfrac{11}3\lambda_1-\tfrac53r_2+\tfrac13r_3,\\
z&=\tfrac{25}3-\tfrac13\lambda_1-\tfrac{11}6r_2-\tfrac13r_3.
\end{aligned}
$$

Every nonbasic variable has nonpositive objective coefficient, so this feasible [simplex basis](../../../../../../simplex-basis.md) is optimal. Setting the nonbasic variables to zero yields

$$
\boxed{\lambda^*=(0,2,1/3),\qquad z^*=25/3.}
$$

Both new basic solutions have strictly positive basic coordinates; neither pivot is degenerate.

The first and fourth dual constraints have positive slacks $8/3$ and $20/3$. [Complementary slackness](../../../../../../complementary-slackness.md) therefore requires $x_1=x_4=0$. Since $\lambda_2,\lambda_3>0$, the second and third primal constraints must be equalities:

$$
2x_2+x_3=4,\qquad 3x_3=1.
$$

Consequently

$$
\boxed{x^*=\left(0,\frac{11}6,\frac13,0\right),\qquad c^Tx^*=\frac{25}3.}
$$

The first primal left side is $10/3\geq3$, so the vector is feasible. Its value matches the feasible dual value, giving a [linear programming optimality certificate](../../../../../../linear-programming-optimality-certificate.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
