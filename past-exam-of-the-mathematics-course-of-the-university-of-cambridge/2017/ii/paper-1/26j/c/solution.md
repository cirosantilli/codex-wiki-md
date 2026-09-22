<h1 id="26j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The chosen non-eventually-one [binary expansion](../../../../../../binary-expansion.md) fixes the ambiguity at dyadic rationals. Its $n$th digit is

$$
\boxed{R_n(x)=\lfloor2^n x\rfloor-2\lfloor2^{n-1}x\rfloor}.
$$

In particular

$$
R_n^{-1}(\{1\})=\bigcup_{j=0}^{2^{n-1}-1}
\left[\frac{2j+1}{2^n},\frac{2j+2}{2^n}\right).
$$

This is a finite union of [Borel sets](../../../../../../borel-set.md); the zero-digit preimage is its complement in $[0,1)$. Since $R_n$ only takes the values zero and one, every Borel preimage is a union of these two [sets](../../../../../../set-split.md). Thus it is Borel measurable. The half-open intervals implement the terminating-zero convention at dyadic endpoints.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26J](../../26j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
