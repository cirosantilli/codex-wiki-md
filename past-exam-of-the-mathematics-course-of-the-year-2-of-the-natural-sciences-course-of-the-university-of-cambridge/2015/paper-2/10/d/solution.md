<h1 id="10/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the left [regular representation](../../../../../regular-representation.md), defined on the ordered basis $(e_I,e_R,\ldots,e_{R^5},e_{m_1},\ldots,e_{m_6})$ by $D_{\rm reg}(g)e_h=e_{gh}$. Reading the $m_4$ row of the original PDF table gives the permutation

$$
(I\ m_4)(R\ m_3)(R^2\ m_2)(R^3\ m_1)(R^4\ m_6)(R^5\ m_5).
$$

Thus an explicit $12\times12$ [permutation matrix](../../../../../permutation-matrix.md), in six-by-six blocks, is

$$
\boxed{D_{\rm reg}(m_4)=\begin{pmatrix}0&P\\P&0\end{pmatrix},\qquad P=\begin{pmatrix}0&0&0&1&0&0\\0&0&1&0&0&0\\0&1&0&0&0&0\\1&0&0&0&0&0\\0&0&0&0&0&1\\0&0&0&0&1&0\end{pmatrix}.}
$$

Each column has its one in the row labelled by the left product; this specifies the convention completely. Since $P^2=I_6$, the full matrix squares to $I_{12}$ and is its own inverse. Therefore for every integer, including negative integers,

$$
\boxed{[D_{\rm reg}(m_4)]^n=\begin{cases}I_{12},&n\text{ even},\\D_{\rm reg}(m_4),&n\text{ odd}.\end{cases}}
$$

This is also immediate from $m_4^2=I$ and the multiplication law for a representation.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
