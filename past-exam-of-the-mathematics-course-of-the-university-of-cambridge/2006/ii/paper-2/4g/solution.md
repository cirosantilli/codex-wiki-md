<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

A [decipherable code](../../../../../decipherable-code.md) is one whose extension to finite strings by concatenation is injective: an encoded string has a unique sequence of source letters. In particular its [codewords](../../../../../codeword.md) are distinct and nonempty. Put $K=\sum_i a^{-s_i}$ and $s_{\max}=\max_i s_i$. For strings of exactly $n$ source letters, let $N_j$ count the encoded strings of length $j$. Unique decipherability gives $N_j\le a^j$, since distinct source strings yield distinct encoded strings. Expanding $K^n$ gives

$$
K^n=\sum_jN_ja^{-j}\le ns_{\max}+1.
$$

Taking $n$th roots and letting $n\to\infty$ proves the [McMillan inequality](../../../../../mcmillan-inequality.md)

$$
\boxed{\sum_i a^{-s_i}\le1.}
$$

Add **$00,01,10$** to the four specified binary words. None of the resulting seven words is a proper suffix of another: the longer words end in $11$, and their shorter terminal strings never equal another of the specified longer words. Thus this is a [suffix code](../../../../../suffix-code.md). Reading from the right determines the last [codeword](../../../../../codeword.md) uniquely; deleting it and repeating proves unique decipherability. Its length sum is $3/4+1/8+1/16+2/32=1$, in agreement with the bound.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
