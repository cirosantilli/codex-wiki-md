<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $V,V',U$ be mutually independent, with $V,V'$ identically distributed. [Entropy submodularity for three independent sums](../../../../../../entropy-submodularity-for-three-independent-sums.md) gives

$$
H(V+V'+U)+H(U)\leq H(V+U)+H(V'+U).
$$

Independent addition cannot decrease discrete entropy, because $H(V+V'+U)\geq H(V+V'+U\mid U)=H(V+V')$. Hence

$$
H(V+V')+H(U)\leq H(U+V)+H(U+V').
$$

Take $U$ to have the distribution of $-X$ and take $V,V'$ to be independent copies of $X$, all mutually independent. Then $U+V$ and $U+V'$ both have the distribution of $X-Y$, whereas $V+V'$ has the distribution of $X+Y$ and $H(U)=H(X)$. Hence

$$
H(X+Y)+H(X)\leq2H(X-Y),
$$

or

$$
H(X+Y)-H(X)\leq2\{H(X-Y)-H(X)\}.
$$

The denominator is nonnegative because conditioning on $Y$ recovers $X$ from $X-Y$, so $H(X-Y)\geq H(X-Y\mid Y)=H(X)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
