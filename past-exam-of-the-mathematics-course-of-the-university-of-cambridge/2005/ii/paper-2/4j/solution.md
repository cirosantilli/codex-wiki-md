<h1 id="4j/solution">Solution</h1>

↑ **Parent:** [4J](../4j.md)

A [binary linear code](../../../../../binary-linear-code.md) of length $n$ is a [vector subspace](../../../../../vector-subspace.md) $C\subseteq\mathbb F_2^n$. The [Hamming weight](../../../../../hamming-weight.md) of a word counts its nonzero coordinates, and the code weight is $w(C)=\min_{0\ne c\in C}\operatorname{wt}(c)$; for a [linear code](../../../../../linear-code.md) this equals its [minimum distance](../../../../../minimum-distance-of-a-code.md). One may assign infinite minimum weight to the zero code when needed.

For length-$n$ codes with $C_2\subseteq C_1$, the [bar product of binary linear codes](../../../../../bar-product-of-binary-linear-codes.md) is

$$
C_1|C_2=\{(u,u+v):u\in C_1,\ v\in C_2\}\subseteq\mathbb F_2^{2n}.
$$

It is a [linear code](../../../../../linear-code.md) because this map from $C_1\oplus C_2$ is linear and injective. For a nonzero [codeword](../../../../../codeword.md), if $v=0$ then $u\ne0$ and its weight is $2\operatorname{wt}(u)\geq2w(C_1)$. If $v\ne0$, every nonzero coordinate of $v$ makes exactly one of the corresponding coordinates of $u,u+v$ nonzero; hence

$$
\operatorname{wt}(u)+\operatorname{wt}(u+v)\geq\operatorname{wt}(v)\geq w(C_2).
$$

Taking the minimum gives

$$
\boxed{w(C_1|C_2)\geq\min\{2w(C_1),w(C_2)\}.}
$$

In fact equality holds when the codes are nonzero: minimum-weight words $(u,u)$ and $(0,v)$ attain the two candidate weights.

## ↑ Ancestors (10)

1. [4J](../4j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
