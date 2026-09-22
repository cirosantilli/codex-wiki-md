<h1 id="19h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because $0\le U\le1$, for fixed $t$ and sufficiently large $n$,

$$
\mathbb P\bigl(n(1-U)\ge t\bigr)
=\begin{cases}
1,&t<0,\\
\mathbb P(U\le1-t/n)=(1-t/n)^n,&t\ge0.
\end{cases}
$$

Therefore

$$
\boxed{h(t)=
\begin{cases}
1,&t<0,\\
e^{-t},&t\ge0.
\end{cases}}
$$

Equivalently, $n(1-\widehat\theta/\theta)$ converges in distribution to an [exponential distribution](../../../../../../exponential-distribution.md) of rate one.

Put $c=\log(1/\alpha)$. The limiting probability

$$
\mathbb P\!\left(n\left(1-\frac{\widehat\theta}{\theta}\right)\le c\right)
\longrightarrow1-e^{-c}=1-\alpha
$$

and the certain inequality $\widehat\theta\le\theta$ suggest the approximate [confidence interval](../../../../../../confidence-interval.md)

$$
\boxed{\left[\widehat\theta,
\frac{n\widehat\theta}{n-\log(1/\alpha)}\right]}.
$$

Since $\mathbb E[\widehat\theta]=n\theta/(n+1)$, its expected length is

$$
\boxed{
\left(\frac{n\theta}{n+1}\right)
\left(\frac{\log(1/\alpha)}{n-\log(1/\alpha)}\right)},
$$

as required.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
