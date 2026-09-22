<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the [Plünnecke-Ruzsa inequality](../../../../../../plunnecke-ruzsa-inequality.md),

$$
|4A|\leq K^4|A|.
$$

Apply the [Ruzsa covering lemma](../../../../../../ruzsa-covering-lemma.md) to $3A$ and $A$. Since $A=-A$, there is a set $X\subseteq3A$ with $|X|\leq K^4$ such that

$$
3A\subseteq X+A-A=X+2A.
$$

Adding $A$ and reusing this inclusion inductively gives

$$
\boxed{mA\subseteq(m-2)X+2A\qquad(m\geq3).}
$$

A sum of $m-2$ members of the fixed set $X$ depends only on the multiplicity of each member. The number of possible multiplicity vectors is at most $m^{|X|}$, and therefore

$$
|(m-2)X|\leq m^{|X|}\leq m^{K^4}.
$$

Since $|2A|\leq K|A|\leq K^m|A|$, it follows that

$$
\boxed{|mA|\leq K^m m^{K^4}|A|.}
$$

For fixed $K$, this differs from the Plünnecke–Ruzsa bound $K^m|A|$ only by a [polynomial](../../../../../../polynomial-split.md) factor in $m$, so both have the same leading [exponential function](../../../../../../exponential-function.md) factor $K^m$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 149](../../../paper-149-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
