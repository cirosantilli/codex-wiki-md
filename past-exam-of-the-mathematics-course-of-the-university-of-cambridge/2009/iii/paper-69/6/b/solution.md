<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Weierstrass M-test](../../../../../../weierstrass-m-test.md) gives a continuous periodic [Weierstrass function](../../../../../../weierstrass-function.md), since $\sum a^{-k}<\infty$. For $5^m\le n<5^{m+1}$, the given best approximant leaves the tail

$$
g-t_n=\sum_{k=m+1}^\infty a^{-k}\cos(5^kx).
$$

Its [supremum norm](../../../../../../supremum-norm.md) is at most the sum of its coefficients, and at $x=0$ all cosine terms equal one, attaining that bound. Consequently

$$
\boxed{E_n(g)=\sum_{k=m+1}^\infty a^{-k}=\frac{a^{-m}}{a-1}.}
$$

Put $\alpha=\ln a/\ln5$. Then $a^{-m}=(5^m)^{-\alpha}$ and $n/5^m\in[1,5)$, giving $E_n(g)\asymp n^{-\alpha}$, with constants depending only on $a$.

For $1<a<5$, part (a) gives $\omega(g,1/n)\le C_an^{-\alpha}$. The [first Jackson theorem for periodic approximation](../../../../../../first-jackson-theorem-for-periodic-approximation.md), $E_n(g)\le C\omega(g,1/n)$, supplies the matching lower bound. Hence the [modulus of continuity](../../../../../../modulus-of-continuity.md) has the precise order

$$
\boxed{\omega(g,\delta)\asymp\delta^{\ln a/\ln5},\qquad1<a<5,\quad\delta\downarrow0.}
$$

At $a=5$, the [inverse theorem for trigonometric approximation](../../../../../../inverse-theorem-for-trigonometric-approximation.md) gives the upper bound $C\delta\ln(1/\delta)$, and part (c) proves the matching lower bound. Thus the [critical Weierstrass modulus](../../../../../../critical-weierstrass-modulus.md) is

$$
\boxed{\omega(g,\delta)\asymp\delta\ln(1/\delta),\qquad a=5.}
$$

To pass from scales $1/n$ to all small $\delta$, use monotonicity of the [modulus of continuity](../../../../../../modulus-of-continuity.md) and adjacent reciprocals, which are comparable to $\delta$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
