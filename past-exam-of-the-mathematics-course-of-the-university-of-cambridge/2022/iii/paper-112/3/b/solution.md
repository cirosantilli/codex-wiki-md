<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Orient the diagram and assign its regions an [Alexander numbering](../../../../../../alexander-numbering.md) with $R_0$ numbered zero. The [abelianization](../../../../../../abelianization.md) $\phi:\pi_1(E_K)\to\langle t\rangle$ sends $a_i$ to $t^{m_i}$, where $m_i$ is the number of $R_i$. Since $R_1$ is adjacent to $R_0$, $m_1=\pm1$.

Form the square matrix

$$
A_1=\left(\phi\!\left(\frac{\partial w_j}{\partial a_i}\right)\right)_{
1\leq j\leq n-1,\ 2\leq i\leq n}
$$

from the [Fox derivatives](../../../../../../fox-calculus.md) with respect to $a_i$ for $i>1$. This is the [Alexander matrix](../../../../../../alexander-matrix.md) with the $a_1$ column deleted. The Fox identity implies that its maximal minors differ by the factors $\phi(a_i)-1$, and the standard presentation of the [Alexander module](../../../../../../alexander-module-of-a-knot.md) therefore gives

$$
\det A_1\doteq\frac{t^{m_1}-1}{t-1}\Delta_K(t)\doteq\Delta_K(t),
$$

because $m_1=\pm1$. Thus $\Delta_K(t)$ is $\det A_1$ up to a unit $\pm t^r$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 112](../../../paper-112-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
