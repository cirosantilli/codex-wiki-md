<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the direct half of the [code-distribution correspondence](../../../../../../code-distribution-correspondence.md), let $L$ be the length function of a binary prefix code and put

$$
K=\sum_x2^{-L(x)}\leq1,
\qquad
R(x)=\frac{2^{-L(x)}}K.
$$

Then $R$ is a [probability mass function](../../../../../../probability-mass-function.md) and

$$
-\log_2R(x)=L(x)+\log_2K\leq L(x).
$$

Thus every prefix code determines a distribution whose ideal description lengths do not exceed the codeword lengths.

Conversely, given a probability mass function $R$, set

$$
L(x)=\left\lceil-\log_2R(x)\right\rceil
$$

for $R(x)>0$. Then $2^{-L(x)}\leq R(x)$, so the [Kraft inequality](../../../../../../kraft-mcmillan-inequality.md) is satisfied. Its converse supplies a binary prefix code with these lengths, and

$$
-\log_2R(x)\leq L(x)<-\log_2R(x)+1.
$$

If real lengths are allowed, the ideal choice $L(x)=-\log_2R(x)$ satisfies Kraft with equality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
