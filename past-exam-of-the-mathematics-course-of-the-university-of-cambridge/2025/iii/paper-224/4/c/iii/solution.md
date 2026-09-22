<h1 id="4/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Relabeling an arbitrary alphabet in decreasing probability order makes part (ii) pointwise:

$$
L^*(x)\leq-\log_2P(x).
$$

It immediately implies

$$
\mathbb P(L^*(X)\geq R)
\leq\mathbb P(-\log_2P(X)\geq R)
$$

and, after taking expectations,

$$
\mathbb E L^*(X)\leq H(X).
$$

This reverses the prefix-code lower bound from part (b). A general one-to-one code need not decode concatenated codewords instantaneously or uniquely, so it is not constrained by Kraft's inequality.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 224](../../../../paper-224-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
