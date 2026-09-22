<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
S=\sum_{T<t\leq2T}\sum_{R<r\leq2R}b_tc_r e(\alpha r^2t^2).
$$

Applying the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in $t$ gives

$$
|S|^2
\leq\|b\|_2^2
\sum_t\left|\sum_r c_re(\alpha r^2t^2)\right|^2
=\|b\|_2^2
\sum_{r_1,r_2}c_{r_1}\overline{c_{r_2}}
\sum_t e\bigl(\alpha t^2(r_1^2-r_2^2)\bigr).
$$

Take absolute values and apply Cauchy-Schwarz to $(r_1,r_2)$. Since $\sum_{r_1,r_2}|c_{r_1}c_{r_2}|^2=\|c\|_2^4$, expanding the remaining square gives

$$
|S|^4
\leq\|b\|_2^4\|c\|_2^4
\sum_{\substack{T<t_1,t_2\leq2T\\R<r_1,r_2\leq2R}}
e\bigl(\alpha(t_1^2-t_2^2)(r_1^2-r_2^2)\bigr).
$$

Taking fourth roots proves the claimed [bilinear quadratic exponential sum fourth-moment bound](../../../../../../bilinear-quadratic-exponential-sum-fourth-moment-bound.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
