<h1 id="3k/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The code $\operatorname{RM}(d,0)$ is the binary repetition code of length $2^d$, while

$$
\operatorname{RM}(d,d)=\mathbb F_2^{\,2^d}
$$

is the full binary code. For $0<r<d$, the [Reed-Muller bar-product recursion](../../../../../../../reed-muller-bar-product-recursion.md) is

$$
\operatorname{RM}(d,r)
=\operatorname{RM}(d-1,r)
\mid\operatorname{RM}(d-1,r-1).
$$

Thus its rank $k(d,r)$ satisfies Pascal's recursion

$$
k(d,r)=k(d-1,r)+k(d-1,r-1),
$$

with the stated boundary values. Therefore

$$
\boxed{k(d,r)=\sum_{j=0}^r\binom dj}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3K](../../../3k.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
