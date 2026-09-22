<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The Shannon lengths are $l_S(a)=\lceil\log_2(1/P(a))\rceil$. Their [Competitive optimality of the Shannon code](../../../../../../competitive-optimality-of-the-shannon-code.md) says that for every binary uniquely decodable code of lengths $l_C$ and every positive integer $k$,

$$
\mathbb P\{l_S(X)\geq l_C(X)+k\}\leq2^{-k+1}.
$$

On this event, $P(X)<2^{-l_C(X)-k+1}$. Summing and applying the [Kraft inequality](../../../../../../kraft-mcmillan-inequality.md) proves

$$
\boxed{\mathbb P\{l_S(X)\geq l_C(X)+k\}
\leq2^{-k+1}\sum_a2^{-l_C(a)}\leq2^{-k+1}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
