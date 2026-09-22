<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The coefficient form of the [Combinatorial Nullstellensatz](../../../../../../combinatorial-nullstellensatz.md) is the following. Let $f\in F[x_1,\ldots,x_n]$ have total degree at most $d_1+\cdots+d_n$, and suppose

$$
[x_1^{d_1}\cdots x_n^{d_n}]f\ne0.
$$

For arbitrary subsets $S_i\subseteq F$ with $|S_i|=d_i+1$, there is an $x\in S_1\times\cdots\times S_n$ such that $f(x)\ne0$.

For the proof, define

$$
\phi_i'(a)=\prod_{b\in S_i\setminus\{a\}}(a-b).
$$

Successive [Lagrange interpolation](../../../../../../lagrange-polynomial.md) in the variables gives the [Alon-Tarsi lemma](../../../../../../alon-tarsi-lemma.md)

$$
[x_1^{d_1}\cdots x_n^{d_n}]f
=\sum_{a_i\in S_i}
\frac{f(a_1,\ldots,a_n)}{\prod_i\phi_i'(a_i)}.
$$

Every denominator is nonzero because the elements of $S_i$ are distinct. If $f$ vanished throughout the product grid, the right side and hence the assumed nonzero coefficient would vanish. This contradiction proves the theorem.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 161](../../../paper-161-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
