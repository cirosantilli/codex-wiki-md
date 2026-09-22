<h1 id="5d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Split the [factorial](../../../../../../factorial.md) at $h$, using $k=p-1-h$:

$$
(p-1)!=h!\prod_{j=h+1}^{p-1}j\equiv h!\prod_{t=1}^{k}(-t)=(-1)^k h!k!\pmod p.
$$

By [Wilson theorem](../../../../../../wilson-s-theorem.md), this is $-1$. Therefore $h!k!\equiv(-1)^{k+1}\pmod p$. If the [prime number](../../../../../../prime-number.md) $p$ is odd, then $h+k=p-1$ is even, so $(-1)^k=(-1)^h$ and

$$
\boxed{h!k!+(-1)^h\equiv0\pmod p.}
$$

For $p=2$, the signs $1$ and $-1$ are identical modulo $2$, and the two possibilities $(h,k)=(0,1),(1,0)$ also give the same result. The [empty product](../../../../../../empty-product.md) convention $0!=1$ includes the endpoint cases. This is the [complementary factorial congruence](../../../../../../complementary-factorial-congruence.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5D](../../5d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
