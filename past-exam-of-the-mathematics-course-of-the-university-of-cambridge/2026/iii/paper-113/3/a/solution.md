<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an indexed open cover $\mathcal U=(U_i)_{i\in I}$ and a sheaf $\mathcal F$, the [Čech cohomology](../../../../../../cech-cohomology.md) cochain groups are

$$
\check C^p(\mathcal U,\mathcal F)
=\prod_{i_0<\cdots<i_p}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_p}).
$$

The differential is the alternating sum of restrictions:

$$
(dc)_{i_0\ldots i_{p+1}}
=\sum_{j=0}^{p+1}(-1)^j
c_{i_0\ldots\widehat{i_j}\ldots i_{p+1}}
\big|_{U_{i_0}\cap\cdots\cap U_{i_{p+1}}}.
$$

Since $d^2=0$, the cohomology

$$
\check H^p(\mathcal U,\mathcal F)
=\ker(d:\check C^p\to\check C^{p+1})/operatorname{im}(d:\check C^{p-1}\to\check C^p)
$$

is well defined.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
