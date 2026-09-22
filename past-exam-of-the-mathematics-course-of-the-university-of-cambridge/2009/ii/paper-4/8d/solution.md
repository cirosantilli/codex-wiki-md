<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

The two [Gamma function](../../../../../gamma-function.md) integrals are absolutely convergent when $\operatorname{Re}\alpha,\operatorname{Re}\beta>0$. Consequently [Fubini theorem](../../../../../fubini-s-theorem.md) gives

$$
\Gamma(\alpha)\Gamma(\beta)
=\int_0^\infty\int_0^\infty x^{\alpha-1}y^{\beta-1}e^{-(x+y)}\,dx\,dy.
$$

Make the [change of variables](../../../../../change-of-variables-formula.md) $u=x+y$, $t=x/(x+y)$, so $x=ut$, $y=u(1-t)$, $u>0$, $0<t<1$, and the Jacobian is $u$. Powers of positive real variables use the real logarithm, so this transformation is also valid for complex exponents. The integral factors as

$$
\left[\int_0^\infty u^{\alpha+\beta-1}e^{-u}\,du\right]
\left[\int_0^1t^{\alpha-1}(1-t)^{\beta-1}\,dt\right].
$$

Both factors converge under the same real-part assumptions. The first is $\Gamma(\alpha+\beta)$, proving the [Beta function](../../../../../beta-function.md) identity

$$
\boxed{\Gamma(\alpha)\Gamma(\beta)=\Gamma(\alpha+\beta)\int_0^1t^{\alpha-1}(1-t)^{\beta-1}\,dt.}
$$

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
