<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In three dimensions, the [Sobolev inequality](../../../../../../sobolev-inequality.md) gives $\lVert v\rVert_{L^6(U)}\leq C_U\lVert v\rVert_{H_0^1(U)}$. Therefore

$$
\lVert w^3\rVert_{L^2(U_T)}^2
=\int_0^T\lVert w(t)\rVert_6^6dt
\leq C_U^6T\lVert w\rVert_{L_t^\infty H_x^1}^6,
$$

and hence

$$
\boxed{\lVert w^3\rVert_{L^2(U_T)}
\leq C_U^3T^{1/2}\lVert w\rVert_{L_t^\infty H_x^1}^3.}
$$

Using $w^3-\widetilde w^3=(w-\widetilde w)(w^2+w\widetilde w+\widetilde w^2)$, the [Holder inequality](../../../../../../holder-inequality.md) and the same Sobolev embedding give at each time

$$
\lVert w^3-\widetilde w^3\rVert_2
\leq C_U^3\lVert w-\widetilde w\rVert_{H^1}
\big(\lVert w\rVert_{H^1}^2+\lVert\widetilde w\rVert_{H^1}^2\big).
$$

Taking the $L^2$ norm in time supplies the required estimate with the factor $T^{1/2}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
