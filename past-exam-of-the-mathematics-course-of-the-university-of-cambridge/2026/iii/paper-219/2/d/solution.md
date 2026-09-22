<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The stated conditional independences give

$$
p(\mathbf d\mid\mathbf x_i,m_i)=
\prod_{s=1}^{N_{\mathrm{sat}}}
\frac1{\sqrt{2\pi\sigma_s^2}}
\exp\left[-\frac{(d_s-x_{si})^2}{2\sigma_s^2}\right].
$$

Thus

$$
\widehat{\mathbb E[m\mid\mathbf d]}=\sum_{i=1}^Km_iw_i,
\qquad
w_i=\frac{\prod_s p(d_s\mid x_{si})}
{\sum_j\prod_s p(d_s\mid x_{sj})}.
$$

The dependence among satellite properties and host mass remains encoded in each jointly simulated row.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
