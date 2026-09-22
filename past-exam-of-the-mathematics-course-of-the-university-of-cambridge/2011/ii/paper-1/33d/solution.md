<h1 id="33d/solution">Solution</h1>

↑ **Parent:** [33D](../33d.md)

On the [tensor product](../../../../../tensor-product.md) state space, the total [angular momentum](../../../../../angular-momentum.md) is $\mathbf J=\mathbf J^{(1)}\otimes I+I\otimes\mathbf J^{(2)}$, conventionally abbreviated $\mathbf J^{(1)}+\mathbf J^{(2)}$. Operators on different factors commute. Define $J_\pm^{(i)}=J_1^{(i)}\pm iJ_2^{(i)}$. Expanding the square gives

$$
\boxed{\mathbf J^2=(\mathbf J^{(1)})^2+(\mathbf J^{(2)})^2+2J_3^{(1)}J_3^{(2)}+J_+^{(1)}J_-^{(2)}+J_-^{(1)}J_+^{(2)}.}
$$

The first three terms commute with $J_3=J_3^{(1)}+J_3^{(2)}$. In a mixed term one subsystem's magnetic quantum number increases and the other's decreases, so its commutator with total $J_3$ is zero. Hence $\boxed{[\mathbf J^2,J_3]=0}$.

Use the standard identities $[J_3,J_\pm]=\pm J_\pm$ and $J_\pm|j,m\rangle=\sqrt{(j\mp m)(j\pm m+1)}|j,m\pm1\rangle$. The PDF has the commutator in the reversed order with unchanged sign and prints $m+1$ also for lowering; these are sign/label slips. The standard identities are consistent with the meaning of raising and lowering and are used here.

Put $s=j_1+j_2$. The unique product state of magnetic quantum number $-s$ is

$$
\boxed{|s,-s\rangle=|j_1,-j_1\rangle|j_2,-j_2\rangle.}
$$

For $j_1,j_2>0$, define the orthonormal product states $|a\rangle=|j_1,-j_1+1\rangle|j_2,-j_2\rangle$ and $|b\rangle=|j_1,-j_1\rangle|j_2,-j_2+1\rangle$. Raising the preceding state gives

$$
|s,-s+1\rangle=\sqrt{\frac{j_1}s}|a\rangle+\sqrt{\frac{j_2}s}|b\rangle.
$$

The normalized orthogonal combination is annihilated by $J_-$, because its two lowering amplitudes cancel. It is consequently the lowest-weight state with $J=s-1$:

$$
\boxed{|s-1,-s+1\rangle=\sqrt{\frac{j_2}s}|a\rangle-\sqrt{\frac{j_1}s}|b\rangle,}
$$

up to an overall phase. For $j_1=3,j_2=1$, the outcome $m_1=-3,m_2=0$ is the $|b\rangle$ component. The [Born rule](../../../../../born-rule.md) therefore gives

$$
\boxed{\mathbb P(m_1=-3,m_2=0\mid|3,-3\rangle)=\frac34.}
$$

## ↑ Ancestors (11)

1. [33D](../33d.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
