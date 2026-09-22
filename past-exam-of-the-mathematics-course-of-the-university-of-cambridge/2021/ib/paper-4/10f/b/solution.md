<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed $(x_1,x_2)$, apply the given one-variable identity to the [smooth function](../../../../../../smooth-function.md)

$$
u(t)=f(x_1,tx_2).
$$

The [chain rule](../../../../../../chain-rule.md) gives

$$
u'(0)=x_2D_2f(x_1,0),
\qquad
u''(t)=x_2^2D_2^2f(x_1,tx_2).
$$

Therefore

$$
f(x_1,x_2)
=f(x_1,0)+x_2D_2f(x_1,0)+x_2^2h(x_1,x_2),
$$

where

$$
\boxed{
h(x_1,x_2)
=\int_0^1(1-t)D_2^2f(x_1,tx_2)\,dt
}.
$$

Every derivative of the integrand is continuous. Repeated [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) therefore shows that $h$ is smooth. This is the [Second-order Hadamard lemma](../../../../../../second-order-hadamard-lemma.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
