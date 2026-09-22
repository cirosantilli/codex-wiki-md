<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Apply the coordinate-replacement proof from part (ii) directly to the [quadratic form](../../../../../../quadratic-form.md)

$$
f(z)=\sum_{i,j}a_{ij}z_iz_j.
$$

The zero diagonal makes $f$ multilinear. For coordinate $i$,

$$
D_i f(z)=\sum_j(a_{ij}+a_{ji})z_j,
$$

and the row and column assumptions imply

$$
\mathbb E(D_i f)^2
=\sum_j(a_{ij}+a_{ji})^2
\leq2\sum_ja_{ij}^2+2\sum_ja_{ji}^2
\leq4.
$$

Every hybrid vector appearing during replacement has independent centered variance-one coordinates with fourth moments at most $9$. The degree-one case of part (i) therefore gives

$$
\mathbb E(D_i f)^4\leq9\bigl(\mathbb E(D_i f)^2\bigr)^2\leq144.
$$

The fourth-order Taylor remainder from replacing coordinate $i$ is at most $(M/12)\mathbb E(D_i f)^4\leq12M$. Summing the $n$ replacement errors yields the stronger estimate

$$
\boxed{\left|\mathbb E\psi\left(\sum_{i,j}a_{ij}X_iX_j\right)
-\mathbb E\psi\left(\sum_{i,j}a_{ij}Y_iY_j\right)\right|
\leq12Mn\leq27Mn.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
