<h1 id="10d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose first that the stated unitary and environment states exist. Preservation of the [inner product](../../../../../../inner-product.md) gives

$$
\langle\phi_0|\phi_1\rangle
=\langle\psi_0|\psi_1\rangle
 \langle e_0|e_1\rangle.
$$

The environment states are normalized, so the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $|\langle e_0|e_1\rangle|\leq1$. Therefore

$$
|\langle\phi_0|\phi_1\rangle|
\leq|\langle\psi_0|\psi_1\rangle|.
$$

Conversely, write

$$
a=\langle\phi_0|\phi_1\rangle,
\qquad b=\langle\psi_0|\psi_1\rangle
$$

and assume $|a|\leq|b|$. If $b\ne0$, put $c=a/b$, so $|c|\leq1$, and choose

$$
|e_0\rangle=|0\rangle,
\qquad
|e_1\rangle=c|0\rangle+\sqrt{1-|c|^2}\,|1\rangle.
$$

Then $\langle e_0|e_1\rangle=c$ and the desired output vectors have inner product $bc=a$, exactly matching the input vectors. If $b=0$, the inequality forces $a=0$, and one may take $|e_0\rangle=|e_1\rangle=|0\rangle$.

In either case the input pair and output pair have the same [Gram matrix](../../../../../../gram-matrix.md). The isometry taking one pair to the other extends to a [unitary matrix](../../../../../../unitary-matrix.md), so the required $U$ exists. Hence

$$
\boxed{
U\text{ exists}
\quad\Longleftrightarrow\quad
|\langle\phi_0|\phi_1\rangle|
\leq|\langle\psi_0|\psi_1\rangle|
},
$$

which is the [environment-assisted two-state pure-state transformation](../../../../../../environment-assisted-two-state-pure-state-transformation.md) criterion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10D](../../10d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
