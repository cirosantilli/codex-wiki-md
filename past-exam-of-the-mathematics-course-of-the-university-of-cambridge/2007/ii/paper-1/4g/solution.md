<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

A [uniquely decodable code](../../../../../decipherable-code.md) is a map whose extension by concatenation to finite strings is [injective](../../../../../injective-function.md). Write $\ell_j$ for its codeword lengths and assume the target alphabet has size $a\ge2$. The [Kraft–McMillan inequality](../../../../../kraft-mcmillan-inequality.md) gives $K=\sum_j a^{-\ell_j}\le1$. The [Gibbs inequality](../../../../../gibbs-inequality.md) says $D(p\Vert q)=\sum_jp_j\log(p_j/q_j)\ge0$ for [probability distributions](../../../../../probability-distribution.md) $p,q$, with the usual convention for zero probabilities.

Set $q_j=a^{-\ell_j}/K$. For [Shannon entropy](../../../../../information-entropy.md) $H(p)=-\sum_jp_j\log p_j$, the [Gibbs inequality](../../../../../gibbs-inequality.md) becomes

$$
0\le-H(p)+(\log a)\sum_jp_j\ell_j+\log K.
$$

Since $\log K\le0$, the [entropy lower bound for prefix codes](../../../../../entropy-lower-bound-for-prefix-codes.md) also applies to this [uniquely decodable code](../../../../../decipherable-code.md):

$$
\boxed{\mathbb E\ell\ge\frac{H(p)-\log K}{\log a}\ge\frac{H(p)}{\log a}.}
$$

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
