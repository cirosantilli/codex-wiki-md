<h1 id="4h/solution">Solution</h1>

↑ **Parent:** [4H](../4h.md)

A [linear code](../../../../../linear-code.md) of length $n$ over $\mathbb F_q$ is a linear subspace $C\subseteq\mathbb F_q^n$. A [parity-check matrix](../../../../../parity-check-matrix.md) $P$ satisfies $C=\ker P$. Its [minimum distance of a code](../../../../../minimum-distance-of-a-code.md) is the least [Hamming distance](../../../../../hamming-distance.md) between distinct codewords, equivalently the least [Hamming weight](../../../../../hamming-weight.md) of a nonzero word, because differences remain in the code.

For the usual binary [bar product of binary linear codes](../../../../../bar-product-of-binary-linear-codes.md), take equal-length binary codes with $C_2\subseteq C_1$ and define

$$
C_1|C_2=\{(u,u+v):u\in C_1,\ v\in C_2\}.
$$

It is linear, of length $2n$ and dimension $\dim C_1+\dim C_2$, since the parametrization is injective. If $v=0$ and the word is nonzero, its weight is $2\operatorname{wt}(u)\ge2d(C_1)$. If $v\ne0$, coordinatewise $\operatorname{wt}(u)+\operatorname{wt}(u+v)\ge\operatorname{wt}(v)\ge d(C_2)$. The words $(u,u)$ with $u$ of minimum nonzero weight and $(0,v)$ with $v$ of minimum weight achieve the two candidate bounds. Thus

$$
\boxed{d(C_1|C_2)=\min\{2d(C_1),d(C_2)\}.}
$$

For a word $(x,y)$, membership is equivalent to $P_1x=0$ and $P_2(x+y)=0$. Consequently a [parity-check matrix of a bar product](../../../../../parity-check-matrix-of-a-bar-product.md) is

$$
\boxed{\begin{pmatrix}P_1&0\\P_2&P_2\end{pmatrix}.}
$$

The same distance argument actually needs only equal block lengths and a common field, not nesting. Over a general field replace the second row block by $(-P_2,P_2)$, so it tests $y-x\in C_2$. The displayed binary construction uses the conventional nesting.

## ↑ Ancestors (10)

1. [4H](../4h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
