<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the [computational basis](../../../../../../computational-basis.md), write

$$
\rho=\frac12\begin{pmatrix}1+s_z&s_x-is_y\\s_x+is_y&1-s_z\end{pmatrix}.
$$

The [Kraus representation](../../../../../../kraus-representation.md) of the [amplitude damping channel](../../../../../../amplitude-damping-channel.md) gives

$$
\Lambda(\rho)=\begin{pmatrix}
\rho_{00}+p\rho_{11}&\sqrt{1-p}\,\rho_{01}\\
\sqrt{1-p}\,\rho_{10}&(1-p)\rho_{11}
\end{pmatrix}.
$$

Reading off its [Bloch vector](../../../../../../bloch-vector.md) gives the [Bloch-vector map of amplitude damping](../../../../../../bloch-vector-map-of-amplitude-damping.md):

$$
\boxed{(s_x,s_y,s_z)\longmapsto
\left(\sqrt{1-p}\,s_x,\sqrt{1-p}\,s_y,p+(1-p)s_z\right).}
$$

Here $0\leq p\leq1$. The shift in $s_z$ shows that this [quantum channel](../../../../../../quantum-channel.md) is not unital unless $p=0$; its fixed ground state lies at the north pole, rather than the center of the [Bloch sphere](../../../../../../bloch-sphere.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
