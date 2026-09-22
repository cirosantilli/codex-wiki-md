# Vector normalization is not linear

↑ **Parent:** [Vector normalization](vector-normalization.md)

[Vector normalization](vector-normalization.md) is not a [linear map](linear-map.md). With $\mathbf e_1=(1,0)$ and $\mathbf e_2=(0,1)$,

$$
\widehat{\mathbf e_1+\mathbf e_2}
=\frac1{\sqrt2}(1,1)
\ne(1,1)=\widehat{\mathbf e_1}+\widehat{\mathbf e_2}.
$$

Consequently, adding individually normalized directions does not generally give the direction of the original [vector sum](vector-sum.md). Compute the intended [vector sum](vector-sum.md) first, then normalize it if it is nonzero. Cancellation is a further boundary case: $v+(-v)=0$ has no normalized direction even though both nonzero summands do. A [numerical algorithm](numerical-algorithm.md) must check that case before dividing by the [norm](norm.md).

## ↑ Ancestors (9)

1. [Vector normalization](vector-normalization.md)
2. [Unit vector](unit-vector.md)
3. [Vector](vector.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
