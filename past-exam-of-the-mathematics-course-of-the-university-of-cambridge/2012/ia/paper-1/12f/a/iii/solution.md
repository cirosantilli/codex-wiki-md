<h1 id="12f/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $R_f,R_g$ be the two [radii of convergence](../../../../../../../radius-of-convergence.md). First take $|x|<t<R_f$, with $t>0$. Absolute convergence at $t$ bounds the terms: $|a_nt^n|\leq M$ for all $n$. Thus

$$
|(n+1)a_{n+1}x^n|\leq\frac Mt(n+1)(|x|/t)^n.
$$

At $x=0$ the right-hand series is finite. Otherwise it converges by the [ratio test](../../../../../../../ratio-test.md), because its limiting ratio is $|x|/t<1$. So the differentiated [power series](../../../../../../../power-series.md) converges absolutely at every interior point of $f$, proving $R_g\geq R_f$. This proof also covers $R_f=\infty$ by choosing a finite $t$ above any given $|x|$; if $R_f=0$, that inequality is automatic.

Conversely, if $0<|x|<R_g$, absolute convergence gives

$$
\sum_{n=1}^\infty|a_n||x|^n
=|x|\sum_{m=0}^\infty\frac{|(m+1)a_{m+1}||x|^m}{m+1}
\leq |x|\sum_{m=0}^\infty|(m+1)a_{m+1}||x|^m<\infty.
$$

The constant term does not affect convergence, and both series converge at zero. Hence $R_f\geq R_g$, including the zero and infinite cases. Therefore **$\boxed{R_f=R_g}$**. This proof uses coefficient estimates, rather than assuming the [termwise differentiation of a power series](../../../../../../../termwise-differentiation-of-a-power-series.md) result whose radius assertion is being established.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [12F](../../../12f.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
