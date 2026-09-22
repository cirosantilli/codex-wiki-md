<h1 id="27j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the [Poisson process](../../../../../../poisson-process.md) $X$ have rate $\lambda$, let $\overline F(t)=\mathbb P(\xi_1>t)$ be the survival function of an inter-renewal time of $N$, and let $\overline H$ be the survival function of the first event time of $Y$. Independence gives

$$
\boxed{\overline H(t)=e^{-\lambda t}\overline F(t)}.
$$

Put

$$
\mu_F=\int_0^\infty\overline F(t)\,dt,
\qquad
\mu_H=\int_0^\infty\overline H(t)\,dt.
$$

At a large time, the excess of $Y$ is the minimum of the excesses of $X$ and $N$. The Poisson excess is an independent rate-$\lambda$ exponential random variable. Applying the renewal excess limit theorem to $N$ and to the assumed renewal process $Y$ gives

$$
\boxed{
\frac1{\mu_H}\int_x^\infty\overline H(y)\,dy
=\frac{e^{-\lambda x}}{\mu_F}
\int_x^\infty\overline F(y)\,dy
}.
$$

Substituting $\overline F(y)=e^{\lambda y}\overline H(y)$ yields the integral equation

$$
\frac1{\mu_H}\int_x^\infty\overline H(y)\,dy
=\frac{e^{-\lambda x}}{\mu_F}
\int_x^\infty e^{\lambda y}\overline H(y)\,dy.
$$

Set $A(x)=\int_x^\infty\overline H(y)dy$ and $c=\mu_H/\mu_F<1$. Differentiating the equation almost everywhere gives

$$
(1-c)\overline H(x)=\lambda A(x).
$$

Since $A'=-\overline H$, it follows that

$$
A'(x)=-\frac{\lambda}{1-c}A(x).
$$

Using $\overline H(0)=1$ shows that $\overline H(x)=e^{-x/\mu_H}$. Thus the first event time of $Y$ is exponential. This is the [exponential first interarrival in a renewal superposition containing a Poisson process](../../../../../../exponential-first-interarrival-in-a-renewal-superposition-containing-a-poisson-process.md) theorem.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [27J](../../27j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
