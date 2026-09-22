<h1 id="30a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Watson lemma](../../../../../../watson-s-lemma.md) states that if

$$
f(t)\sim\sum_{n=0}^{\infty}a_nt^{\lambda_n-1}
\quad(t\downarrow0),
\qquad
0<\lambda_0<\lambda_1<\cdots,
$$

and the [Laplace integral](../../../../../../laplace-integral.md) has suitable growth control away from zero, then

$$
\int_0^b e^{-xt}f(t)\,dt
\sim\sum_{n=0}^{\infty}
a_n\Gamma(\lambda_n)x^{-\lambda_n}
\quad(x\to+\infty).
$$

The [Taylor series](../../../../../../taylor-series.md) of the amplitude is

$$
\sin(t^2)
=\sum_{k=0}^{\infty}\frac{(-1)^k}{(2k+1)!}t^{4k+2}.
$$

Termwise application of Watson lemma therefore gives the [asymptotic expansion](../../../../../../asymptotic-expansion.md)

$$
\boxed{
I(x)\sim
\sum_{k=0}^{\infty}
\frac{(-1)^k\Gamma(4k+3)}{(2k+1)!x^{4k+3}}
=\frac2{x^3}-\frac{120}{x^7}
+\frac{30240}{x^{11}}-\cdots.}
$$

In particular, the leading asymptotic approximation is $I(x)\sim2x^{-3}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30A](../../30a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
