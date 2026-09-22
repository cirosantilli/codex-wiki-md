<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

Let

$$
x=\sqrt[3]2+\sqrt[3]3.
$$

If $x$ were [rational](../../../../../rational-number.md), then

$$
x^3=5+3x\sqrt[3]6
$$

would make $\sqrt[3]6=(x^3-5)/(3x)$ rational. But if $\sqrt[3]6=a/b$ in lowest terms, then $a^3=6b^3$, which is impossible by [unique prime factorization](../../../../../fundamental-theorem-of-arithmetic.md): the exponent of $2$ on the two sides is respectively a multiple of three and one more than a multiple of three. Therefore

$$
\boxed{\sqrt[3]2+\sqrt[3]3\text{ is irrational}}.
$$

Use the given [convergent series](../../../../../convergent-series.md)

$$
e-e^{-1}=2\sum_{n=0}^{\infty}\frac1{(2n+1)!}.
$$

Suppose this number were $a/b\in\mathbb Q$. Choose $N$ large enough that $b\mid(2N+1)!$. Multiplication by $(2N+1)!$ makes both the rational number and the partial sum through $n=N$ integers. Their difference

$$
R_N
=2(2N+1)!\sum_{n=N+1}^{\infty}\frac1{(2n+1)!}
$$

would therefore be an integer. It is positive, while

$$
0<R_N
\leq2\sum_{j=1}^{\infty}\frac1{(2N+2)^{2j}}
<1
$$

for sufficiently large $N$, a contradiction. Hence

$$
\boxed{e-e^{-1}\text{ is irrational}}.
$$

A [transcendental number](../../../../../transcendental-number.md) is a complex number that is not a root of any nonzero polynomial with rational, equivalently integer, coefficients. Let

$$
y=ae+be^{-1},
\qquad (a,b)\ne(0,0).
$$

If $a\ne0$ and $y$ were an [algebraic number](../../../../../algebraic-number.md), then $e$ would satisfy

$$
aX^2-yX+b=0
$$

over the algebraic extension $\mathbb Q(y)$. By [transitivity of algebraic extensions](../../../../../transitivity-of-algebraic-extensions.md), $e$ would be algebraic over $\mathbb Q$, contradicting its transcendence. If $a=0$, then $b\ne0$ and $e=b/y$ would again be algebraic. Thus

$$
\boxed{ae+be^{-1}\text{ is transcendental}}.
$$

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
