<h1 id="20g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
\theta=\frac{1+\sqrt{-p}}2\in\mathcal O_L.
$$

Its minimal polynomial is $X^2-X+m$, and the [algebraic norm](../../../../../../algebraic-norm.md) gives

$$
N_{L/\mathbb Q}(n+\theta)=n^2+n+m=:N.
$$

Suppose that $N$ is composite and choose a prime divisor $q\leq\sqrt N<m$. Since $X^2-X+m$ has the root $-n$ modulo $q$, the ideal

$$
\mathfrak q=(q,n+\theta)
$$

is a [prime ideal](../../../../../../prime-ideal.md) of [ideal norm](../../../../../../ideal-norm.md) $q$. The triviality of the [ideal class group](../../../../../../ideal-class-group.md) makes $\mathfrak q=(\beta)$ principal, so $|N_{L/\mathbb Q}(\beta)|=q$.

The [ring of integers of a quadratic field](../../../../../../ring-of-integers-of-a-quadratic-field.md) consists of elements

$$
\beta=\frac{a+b\sqrt{-p}}2,
\qquad a\equiv b\pmod2,
$$

whose norm is $(a^2+pb^2)/4$. If $b=0$, this norm is a square and cannot be the prime $q$. If $b\ne0$, then

$$
q=\frac{a^2+pb^2}{4}\geq\frac p4=m-\frac14,
$$

and integrality gives $q\geq m$, again a contradiction. Therefore the [Euler prime-generating quadratic from class number one](../../../../../../euler-prime-generating-quadratic-from-class-number-one.md) yields

$$
\boxed{\ n^2+n+m\text{ is prime}.\ }
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20G](../../20g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
