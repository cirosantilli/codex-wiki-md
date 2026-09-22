<h1 id="9f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [ratio test](../../../../../../ratio-test.md) says that if

$$
\limsup_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|=L<1,
$$

then $\sum a_n$ converges absolutely. If the ratio has a [limit](../../../../../../limit-of-a-function.md) $L>1$, the [series](../../../../../../series-mathematics.md) diverges.

For the first assertion, choose $q$ with $L<q<1$. For all sufficiently large $n$,

$$
|a_{n+1}|\leq q|a_n|.
$$

Iteration bounds the tail by a constant multiple of the convergent geometric [series](../../../../../../series-mathematics.md) $\sum q^n$. If $L>1$, choose $q$ with $1<q<L$. Eventually $|a_{n+1}|\geq q|a_n|$, so $a_n$ cannot tend to zero; the [series](../../../../../../series-mathematics.md) therefore diverges.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
