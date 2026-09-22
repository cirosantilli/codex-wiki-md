<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose an ordering of the index set $I$. The degree-$q$ [Čech cochain group](../../../../../../cech-cochain-group.md) is

$$
\check C^q(\mathcal U,\mathcal F)
=\prod_{i_0<\cdots<i_q}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_q}).
$$

For $s=(s_{i_0\cdots i_q})$, the [Čech coboundary](../../../../../../cech-coboundary.md) is the alternating sum of restrictions

$$
(\delta s)_{i_0\cdots i_{q+1}}
=\sum_{j=0}^{q+1}(-1)^j
s_{i_0\cdots\widehat{i_j}\cdots i_{q+1}}
\big|_{U_{i_0}\cap\cdots\cap U_{i_{q+1}}}.
$$

The identity $\delta^2=0$ makes this the [Čech cochain complex](../../../../../../cech-cochain-complex.md), and the required [Čech cohomology](../../../../../../cech-cohomology.md) is

$$
\boxed{\check H^q(\mathcal U,\mathcal F)=\ker(\delta:\check C^q\to\check C^{q+1})/\operatorname{im}(\delta:\check C^{q-1}\to\check C^q).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
