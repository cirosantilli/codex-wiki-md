<h1 id="12f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Taylor's theorem about $1$ gives, for some $\xi\in[t,1]$,

$$
G_X(t)=1-\mu(1-t)+\frac12G_X''(\xi)(1-t)^2.
$$

Since $G_X''$ is nondecreasing and

$$
G_X''(1)=\mathbb E[X(X-1)]=\sigma^2+\mu^2-\mu=:A,
$$

the stated inequality follows. At the fixed point $d<1$,

$$
0\leq(1-d)\left[1-\mu+\frac A2(1-d)\right].
$$

Therefore the [quadratic Galton-Watson extinction bound](../../../../../../quadratic-galton-watson-extinction-bound.md) is

$$
d\leq d^*:=1-\frac{2(\mu-1)}{\sigma^2+\mu^2-\mu}<1.
$$

The denominator is at least $2(\mu-1)$ because $X$ is integer-valued and $\mathbb E[(X-1)(X-2)]\geq0$, so $d^*\geq0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [12F](../../12f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
