<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The $2^n$ increments are independent [normal random variables](../../../../../../gaussian-random-variable.md), each distributed as $2^{-n/2}B_1$. Their squared means are $2^{-n}$ and, using the permitted [variance](../../../../../../variance-split.md), their squared variances are $2\cdot2^{-2n}$. [Independence](../../../../../../independent-random-variables.md) therefore gives

$$
\mathbb E[B]_n=2^n2^{-n}=1,
\qquad \operatorname{var}([B]_n)=2^n\,2\cdot2^{-2n}=2^{1-n}.
$$

Consequently **the dyadic quadratic variation converges to one**:

$$
\boxed{\mathbb E\bigl([B]_n-1\bigr)^2=2^{1-n}\longrightarrow0,
\qquad [B]_n\longrightarrow1\text{ in }L^2.}
$$

This is [dyadic quadratic variation of Brownian motion](../../../../../../dyadic-quadratic-variation-of-brownian-motion.md) on the time interval of length one. The calculation requires [independence](../../../../../../independent-random-variables.md) only within each partition; increments from different resolutions need not be independent.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
