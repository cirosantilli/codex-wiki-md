<h1 id="2/i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every member of the [typical set](../../../../../../../typical-set.md) has probability at least $2^{-n(H(X)+\varepsilon)}$. Summing these probabilities gives

$$
1\geq\sum_{x^n\in T_\varepsilon^{(n)}}p(x^n)
\geq|T_\varepsilon^{(n)}|\,2^{-n(H(X)+\varepsilon)},
$$

so

$$
\boxed{|T_\varepsilon^{(n)}|\leq2^{n(H(X)+\varepsilon)}}.
$$

The upper bound itself holds at every block length. For sufficiently large $n$, the high-probability property also gives the companion lower bound

$$
1-\delta\leq\mathbb P(T_\varepsilon^{(n)})
\leq|T_\varepsilon^{(n)}|\,2^{-n(H(X)-\varepsilon)},
$$

hence $|T_\varepsilon^{(n)}|\geq(1-\delta)2^{n(H(X)-\varepsilon)}$. Together these are the [typical-set cardinality bounds](../../../../../../../typical-set-cardinality-bounds.md) underlying [Shannon source coding theorem](../../../../../../../shannon-s-source-coding-theorem.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [I](../../i.md)
3. [2](../../../2.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
