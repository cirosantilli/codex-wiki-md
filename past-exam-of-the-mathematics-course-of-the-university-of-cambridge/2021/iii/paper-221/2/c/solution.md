<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [homogeneous treatment effect](../../../../../../homogeneous-treatment-effect.md) and consistency imply

$$
Y-\beta_0A=Y(0)=:R.
$$

Instrument validity gives $Z\mathrel\perp R\mid X$.

If Assumption 1 holds, put $V=R-\alpha_0X$. Then $\mathbb E[V\mid X]=0$, so conditional instrument independence gives

$$
\mathbb E[VZ]=0,
\qquad
\mathbb E[VX]=0.
$$

Consequently both population estimating equations vanish at $(\beta_0,\alpha_0)$ for any probability limit of $\widehat\gamma$.

If Assumption 2 holds, choose the linear-projection coefficient

$$
\alpha_*=\frac{\mathbb E[RX]}{\mathbb E[X^2]}.
$$

Then $\mathbb E[(R-\alpha_*X)X]=0$, while

$$
\begin{aligned}
\mathbb E[(R-\alpha_*X)(Z-cX)]
&=\mathbb E[(R-\alpha_*X)\{Z-\mathbb E[Z\mid X]\}]\\
&\quad+(\gamma_0-c)\mathbb E[(R-\alpha_*X)X]=0.
\end{aligned}
$$

The first term is zero by conditional instrument independence and the second by the definition of $\alpha_*$. Thus $(\beta_0,\alpha_*)$ solves the population equations. Under the nonsingularity condition from part b, the root is unique, so standard [estimating equation](../../../../../../estimating-equation.md) consistency proves

$$
\widehat\beta\xrightarrow{p}\beta_0
$$

whenever either Assumption 1 or Assumption 2 holds. This is [double robustness](../../../../../../double-robustness.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
