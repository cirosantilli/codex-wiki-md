<h1 id="2/2/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a smooth radial function that decays at infinity,

$$
r^{d-1}|u(r)|^2
=-\int_r^\infty\frac d{ds}\bigl(s^{d-1}|u(s)|^2\bigr),ds
\leq2\int_r^\infty s^{d-1}|u(s)||u'(s)|,ds.
$$

The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) therefore yields the [Radial Sobolev inequality](../../../../../../../radial-sobolev-inequality.md)

$$
|u(r)|^2\leq\frac2{r^{d-1}}\|u\|_2\|\nabla u\|_2,
$$

up to the harmless common normalization of surface measure. Taking the supremum over $r\geq R$ gives the claimed estimate; density extends it from smooth radial functions to every $u\in H^1_r$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
