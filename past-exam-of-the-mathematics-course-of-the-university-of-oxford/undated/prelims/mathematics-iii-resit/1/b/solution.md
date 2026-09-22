<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [product rule](../../../../../../product-rule.md) gives $y'=x^nz'+nx^{n-1}z$ and $y''=x^nz''+2nx^{n-1}z'+n(n-1)x^{n-2}z$. On an [interval](../../../../../../interval-mathematics.md) avoiding $x=0$, substitution and division by $x^{n+2}$ give

$$
z''+\left(2+\frac{2n+4}{x}\right)z'
+\left(2+\frac{2n+4}{x}+\frac{n^2+3n+2}{x^2}\right)z=0.
$$

For a [constant-coefficient differential equation](../../../../../../constant-coefficient-differential-equation.md), the coefficient of $z'$ forces $2n+4=0$. At $n=-2$, the remaining coefficient $n^2+3n+2$ also vanishes. Thus

$$
\boxed{n=-2,\qquad z''+2z'+2z=0.}
$$

The [characteristic equation of a constant-coefficient differential equation](../../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is $r^2+2r+2=0$, with [complex conjugate](../../../../../../complex-conjugate.md) [roots of a polynomial](../../../../../../root-of-a-polynomial.md) $-1\pm i$. Its real solutions $e^{-x}\cos x$ and $e^{-x}\sin x$ are [linearly independent](../../../../../../linear-independence.md). Therefore the [general solution](../../../../../../general-solution.md) is

$$
\boxed{y(x)=\frac{e^{-x}}{x^2}(A\cos x+B\sin x),\qquad x\ne0.}
$$

The constants can be chosen independently on the two sides of the singular point. The [power substitution reducing a differential equation to constant coefficients](../../../../../../power-substitution-reducing-a-differential-equation-to-constant-coefficients.md) here is invertible wherever $x\ne0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Mathematics III resit](../../../mathematics-iii-resit-split.md)
4. [Prelims](../../../split.md)
5. [Undated](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
