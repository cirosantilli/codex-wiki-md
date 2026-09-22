<h1 id="11f/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**True.** First choose polynomials $Q_n\to f$ uniformly by the [Weierstrass approximation theorem](../../../../../../../weierstrass-approximation-theorem.md). Let $L_1,\ldots,L_m$ be the [Lagrange interpolation polynomials](../../../../../../../lagrange-polynomial.md) for the nodes $x_1,\ldots,x_m$, so $L_j(x_i)=\delta_{ij}$. Set

$$
P_n(x)=Q_n(x)+\sum_{j=1}^m\bigl(f(x_j)-Q_n(x_j)\bigr)L_j(x).
$$

Then $P_n(x_j)=f(x_j)$ for every $j$, while

$$
\|P_n-f\|_\infty
\leq\|Q_n-f\|_\infty
\left(1+\sum_{j=1}^m\|L_j\|_\infty\right)\longrightarrow0.
$$

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [11F](../../../11f.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
