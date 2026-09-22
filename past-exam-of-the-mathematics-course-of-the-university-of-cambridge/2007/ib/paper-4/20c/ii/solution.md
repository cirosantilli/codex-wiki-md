<h1 id="20c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The amended payoff is $P_{\mathrm{new}}=P+3x_3$. Using the previous [simplex dictionary](../../../../../../simplex-dictionary.md),

$$
P_{\mathrm{new}}=8+\tfrac12x_3-\tfrac43z_1-\tfrac16z_2.
$$

Thus $x_3$ enters. The positive pivot-column coefficients give ratios $3/(1/2)=6$ from $x_2$ and $(29/2)/10=29/20$ from $z_3$; the coefficient $-3/2$ in the $x_1$ row gives no bound. The [simplex ratio test](../../../../../../simplex-ratio-test.md) makes $z_3$ leave. Dividing that row by $10$ and eliminating $x_3$ gives

$$
\begin{aligned}
x_1+\tfrac{19}{120}z_1+\tfrac{17}{120}z_2+\tfrac3{20}z_3&=\tfrac{107}{40},\\
x_2+\tfrac9{40}z_1+\tfrac7{40}z_2-\tfrac1{20}z_3&=\tfrac{91}{40},\\
x_3+\tfrac{13}{60}z_1-\tfrac1{60}z_2+\tfrac1{10}z_3&=\tfrac{29}{20},\\
P_{\mathrm{new}}+\tfrac{173}{120}z_1+\tfrac{19}{120}z_2+\tfrac1{20}z_3&=\tfrac{349}{40}.
\end{aligned}
$$

The positive objective-row coefficients and nonnegative [slack variables](../../../../../../slack-variable.md) prove optimality at $z_1=z_2=z_3=0$. Therefore

$$
\boxed{x=(\tfrac{107}{40},\tfrac{91}{40},\tfrac{29}{20}),\qquad\min(2x_1-3x_2-5x_3)=-\tfrac{349}{40}.}
$$

All three constraints are equalities at this point. Strict positivity of the three objective-row coefficients also forces every optimal point to have all three slacks zero; the displayed dictionary then makes the optimizer unique.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [20C](../../20c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
