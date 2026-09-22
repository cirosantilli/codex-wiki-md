<h1 id="23h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an [integrable](../../../../../../lebesgue-integrable-function.md) function $f:\mathbb R^n\to\mathbb C$, the [Lebesgue differentiation theorem](../../../../../../lebesgue-differentiation-theorem.md) states that

$$
\lim_{r\downarrow0}\frac1{\lambda(B(x,r))}
\int_{B(x,r)}|f(y)-f(x)|\,d\lambda(y)=0
$$

for [almost everywhere](../../../../../../almost-everywhere.md) $x\in\mathbb R^n$. In particular,

$$
\lim_{r\downarrow0}\frac1{\lambda(B(x,r))}
\int_{B(x,r)}f(y)\,d\lambda(y)=f(x)
$$

at every [Lebesgue point](../../../../../../lebesgue-point.md) of $f$.

Almost every $x\in\mathbb R$ is a Lebesgue point of $g$. At such an $x$, for $t>0$,

$$
\left|\frac{G(x+t)-G(x)}t-g(x)\right|
\leq\frac1t\int_x^{x+t}|g(y)-g(x)|\,d\lambda(y)\longrightarrow0.
$$

For $t<0$, the same estimate over $[x+t,x]$ gives the identical [limit](../../../../../../limit-of-a-function.md). Therefore

$$
\boxed{G'(x)=g(x)}
$$

at every Lebesgue point of $g$, so $G$ is [differentiable](../../../../../../differentiable-function.md) $\lambda$-almost everywhere. This is the [differentiation of an indefinite Lebesgue integral](../../../../../../differentiation-of-an-indefinite-lebesgue-integral.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [23H](../../23h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
