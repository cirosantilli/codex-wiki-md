<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Combined interior and boundary [elliptic regularity](../../../../../../elliptic-regularity.md) for the Dirichlet Laplacian on a smooth bounded domain states that, for every integer $k\geq0$,

$$
\|u\|_{H^{k+2}(\Omega)}
\leq C_k\|f\|_{H^k(\Omega)}
$$

when $\Delta u=f$ and $u$ has zero boundary trace. More generally one first has an additional $\|u\|_{L^2}$ term, which uniqueness and the Poincare inequality remove here.

For the shifted equation, write $\Delta u=f+u$. The weak estimate gives $u\in H^1$. Applying the displayed estimate first with an $L^2$ right side gives $u\in H^2$. Repeating,

$$
f\in H^k,\quad u\in H^j
\quad\Longrightarrow\quad
u\in H^{\min(k,j)+2},
$$

until $u\in H^{k+2}$. The lower-order term is controlled at each stage, yielding

$$
\|u\|_{H^{k+2}}\leq C_k\|f\|_{H^k}.
$$

This is [boundary elliptic regularity for the shifted Dirichlet Laplacian](../../../../../../boundary-elliptic-regularity-for-the-shifted-dirichlet-laplacian.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
