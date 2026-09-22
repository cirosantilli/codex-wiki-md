<h1 id="6h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The joint density depends on the sample through

$$
\sum_{i=1}^nX_i^2,
$$

not merely through $\sum_i|X_i|$. For example, after padding with zeros when $n>2$, take

$$
x=(1,1,0,\ldots,0),
\qquad
y=(2,0,0,\ldots,0).
$$

Both samples have sum of absolute values $2$, but

$$
\frac{p_\sigma(x)}{p_\sigma(y)}
=\exp\left(\frac1{\sigma^2}\right),
$$

which depends on $\sigma$. The likelihood-ratio necessary condition for sufficiency fails, so

$$
\boxed{\sum_{i=1}^n|X_i|\text{ is not sufficient}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6H](../../6h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
