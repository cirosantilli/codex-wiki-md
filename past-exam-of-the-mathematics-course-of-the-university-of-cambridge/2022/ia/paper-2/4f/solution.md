<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

Expanding around the [expected value](../../../../../expected-value.md) $\mu$,

$$
G(a)=\mathbb E[(X-\mu+\mu-a)^2]
=\mathbb E[(X-\mu)^2]+(\mu-a)^2,
$$

because $\mathbb E[X-\mu]=0$. Therefore

$$
\boxed{G(a)=\sigma^2+(\mu-a)^2\geq\sigma^2},
$$

with equality exactly when $a=\mu$.

For the absolute loss,

$$
H(a)=\int_{-\infty}^a(a-x)f(x)\,dx
+\int_a^\infty(x-a)f(x)\,dx.
$$

Leibniz differentiation gives, with $F(a)=\int_{-\infty}^af(x)\,dx$,

$$
H'(a)=F(a)-(1-F(a))=2F(a)-1.
$$

Thus $H$ decreases while $F(a)<1/2$ and increases while $F(a)>1/2$. It is minimized at any [median](../../../../../median.md), characterized in the continuous case by

$$
\boxed{\int_{-\infty}^af(x)\,dx=\frac12}.
$$

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
