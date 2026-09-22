<h1 id="1e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the [composite number](../../../../../../composite-number.md) as $n=ab$, with $2\le a\le b<n$. If $a<b$, both $a$ and $b$ occur as distinct factors of the [factorial](../../../../../../factorial.md) $(n-1)!$, so their product $n$ divides that [factorial](../../../../../../factorial.md).

If $a=b$, then $n=a^2$ and $n>4$ implies $a\ge3$. Both $a$ and $2a$ are distinct factors in $(n-1)!$, because $2a\le a^2-1$. Their product is $2n$, so again $n$ divides the [factorial](../../../../../../factorial.md). Hence

$$
\boxed{(n-1)!\equiv0\pmod n\quad\text{for every composite }n>4.}
$$

The exception $n=4$ matters: its [factorial](../../../../../../factorial.md) $3!=6$ is not divisible by $4$. This argument handles perfect squares without incorrectly counting the same factor twice.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1E](../../1e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
