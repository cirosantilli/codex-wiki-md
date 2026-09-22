<h1 id="18j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a monic [polynomial](../../../../../../polynomial-split.md) with roots $r_1,\ldots,r_n$, its discriminant is

$$
\operatorname{Disc}(f)=\prod_{i<j}(r_i-r_j)^2.
$$

Here $\operatorname{Disc}(g)=(u^3-v^3)^2$. Both $u^3-v^3$ and the Vandermonde product in the $\alpha_i$ are alternating homogeneous cubics. Evaluation at $(\alpha_1,\alpha_2,\alpha_3)=(0,1,-1)$ fixes the constant and gives

$$
 (u^3-v^3)^2=-27\prod_{i<j}(\alpha_i-\alpha_j)^2=-27\operatorname{Disc}(f).
$$

Using $\alpha_1+\alpha_2+\alpha_3=0$, $\sum_{i<j}\alpha_i\alpha_j=a$, and $\alpha_1\alpha_2\alpha_3=-b$, direct expansion gives

$$
uv=-3a,\qquad u^3+v^3=-27b.
$$

Consequently

$$
g(X)=X^2+27bX-27a^3,
$$

and

$$
\operatorname{Disc}(g)=729b^2+108a^3=-27(-4a^3-27b^2).
$$

Thus

$$
\boxed{\operatorname{Disc}(f)=-4a^3-27b^2}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18J](../../18j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
