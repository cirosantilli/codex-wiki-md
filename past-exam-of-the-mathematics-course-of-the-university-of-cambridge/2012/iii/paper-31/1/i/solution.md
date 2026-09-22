<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $V_m=\det[x_i^{j-1}]_{i,j=1}^m$. It is an [alternating polynomial](../../../../../../alternating-polynomial.md): exchanging two variables exchanges two rows of the [Vandermonde matrix](../../../../../../vandermonde-matrix.md) and reverses its [determinant](../../../../../../determinant.md). Hence $V_m$ vanishes whenever $x_k=x_l$, so each factor $x_l-x_k$ divides it. The distinct linear factors are pairwise [coprime polynomials](../../../../../../coprime-polynomials.md), and their product therefore divides $V_m$. Both have total degree $0+1+\cdots+(m-1)=m(m-1)/2$, so

$$
V_m=C_m\prod_{k<l}(x_l-x_k).
$$

The coefficient of $x_m^{m-1}$ in the [determinant](../../../../../../determinant.md) is $V_{m-1}$, by expansion along its last row. The same coefficient in the product is $\prod_{k<l<m}(x_l-x_k)$. Thus $C_m=C_{m-1}$, and $C_1=1$. Consequently the [Vandermonde determinant](../../../../../../vandermonde-determinant.md) identity is

$$
\boxed{\det[x_i^{j-1}]_{i,j=1}^m=\prod_{1\leq k<l\leq m}(x_l-x_k).}
$$

This is a [polynomial](../../../../../../polynomial-split.md) identity, including repeated coordinates; no division by a possibly zero numerical Vandermonde product is needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
