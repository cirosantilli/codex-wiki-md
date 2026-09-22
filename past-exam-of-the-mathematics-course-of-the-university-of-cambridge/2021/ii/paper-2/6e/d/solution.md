<h1 id="6e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $f_n=n^2$, the birth increment is $2n+1$, while

$$
f_n-f_{n-2}=n^2-(n-2)^2=4n-4.
$$

With $D=2d$, the generator identity gives

$$
\boxed{
\frac d{dt}\langle n^2\rangle
=b(2\mu+1)-4d(\langle n^2\rangle-\mu)-2dp_1}.
$$

At stationarity $\mu=b/(2d)$, and solving this equation for the [variance](../../../../../../variance-split.md) yields

$$
\sigma^2=\langle n^2\rangle-\mu^2
=\frac{3b}{4d}-\frac{p_1}{2}.
$$

For $b,d>0$ the chain is irreducible on the nonnegative integers, so its stationary distribution has $0<p_1<1$. Therefore

$$
\boxed{\frac{3b}{4d}-\frac12<\sigma^2<\frac{3b}{4d}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6E](../../6e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
