<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [Itô product rule](../../../../../../ito-product-rule.md) and the [quadratic covariation](../../../../../../quadratic-covariation.md) rule for a [stochastic integral](../../../../../../stochastic-integral.md). The [finite variation](../../../../../../total-variation-of-a-function.md) [consumption](../../../../../../consumption.md) term has zero [quadratic covariation](../../../../../../quadratic-covariation.md) with $Z$, so

$$
d[Z,X]_t=\sum_iH_t^i\,d[Z,P^i]_t.
$$

Using $X=H\cdot P$ and the wealth equation,

$$
\begin{aligned}d(ZX)&=Z\,dX+X\,dZ+d[Z,X]\\&=H\cdot(Z\,dP+P\,dZ+d[Z,P])-Zc\,dt.
\end{aligned}
$$

Thus the [deflated wealth equation with consumption](../../../../../../deflated-wealth-equation-with-consumption.md) is

$$
\boxed{d(Z_tX_t)=H_t\cdot d(Z_tP_t)-Z_tc_t\,dt.}
$$

No [finite variation](../../../../../../total-variation-of-a-function.md) assumption on $H$ is needed: the self-financing equation and the stochastic-integral [quadratic covariation](../../../../../../quadratic-covariation.md) rule already incorporate the [portfolio](../../../../../../investment-portfolio.md)'s financing constraint.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
