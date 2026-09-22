<h1 id="13g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For nonnegative integers $m,n$, put $B(z)=z^m[(z-a)/(1-\bar a z)]^n$. Since $|a|<1$, the denominator has no zero on or inside the unit circle. On $|z|=1$,

$$
|z-a|^2=1-z\bar a-\bar z a+|a|^2=|1-\bar a z|^2,
$$

so $|B(z)|=1$. Consequently $|-a|<|B(z)|$, and [Rouché's theorem](../../../../../../rouche-s-theorem.md) gives the same interior zero count for $B-a$ as for $B$. The latter has $m$ zeros at zero and $n$ at $a$, with the multiplicities combining when $a=0$. Therefore

$$
\boxed{B(z)-a\text{ has }m+n\text{ zeros in }|z|<1\text{, counting multiplicity}}.
$$

This is the [interior zero count for a finite Blaschke product minus a constant](../../../../../../interior-zero-count-for-a-finite-blaschke-product-minus-a-constant.md). If $m+n=0$, the nonzero constant $1-a$ has zero zeros, so the same conclusion includes that endpoint case.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13G](../../13g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
