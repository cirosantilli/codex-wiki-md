<h1 id="17/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The product in the integrand simplifies to $\sin x\cos^3x$ below its upper endpoint. With the [integration by substitution](../../../../../integration-by-substitution.md) $t=\cos x$, the limits become $c$ and zero and $dt=-\sin x\,dx$. Therefore

$$
I=-\int_c^0t^3\,dt=\int_0^ct^3\,dt=J,
\qquad\boxed{I=J=\frac{c^4}{4}.}
$$

Although the [tangent function](../../../../../tangent-function.md) itself is undefined at the upper endpoint, the product has a zero [limit](../../../../../limit-of-a-function.md) there, so its continuous extension, or its [improper integral](../../../../../improper-integral.md), gives this same result.

To obtain $J$ directly from a [Riemann sum](../../../../../riemann-sum.md), divide $[0,c]$ into $n$ equal pieces of width $c/n$ and use right endpoints $t_k=kc/n$. The sum is

$$
\sum_{k=1}^n\left(\frac{kc}{n}\right)^3\frac cn
=\frac{c^4}{n^4}\frac{n^2(n+1)^2}{4}
=\frac{c^4}{4}\left(1+\frac1n\right)^2.
$$

The integrand is continuous, so the [limit](../../../../../limit-of-a-function.md) of these [Riemann sums](../../../../../riemann-sum.md) is its [definite integral](../../../../../definite-integral.md), namely $c^4/4$, agreeing with the [antiderivative](../../../../../antiderivative.md) calculation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [17](../../17.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
