<h1 id="19i/solution">Solution</h1>

↑ **Parent:** [19I](../19i.md)

The [special unitary group](../../../../../special-unitary-group.md) is $\mathrm{SU}(2)=\{g\in M_2(\mathbb C):g^*g=I,\ \det g=1\}$. The [special orthogonal group](../../../../../special-orthogonal-group.md) is $\mathrm{SO}(3)=\{R\in M_3(\mathbb R):R^TR=I,\ \det R=1\}$. [Conjugation](../../../../../conjugation.md) $A\mapsto gAg^{-1}$ preserves [trace](../../../../../matrix-trace.md) and skew-Hermiticity: for unitary $g$, $(gAg^{-1})^*=gA^*g^{-1}=-gAg^{-1}$. It therefore defines the representation on the real space $V$ described in the following parts. The bar over the transpose in the PDF is essential; the condition is $A+A^*=0$, not ordinary antisymmetry over the [complex numbers](../../../../../complex-number.md).

An [orthonormal basis](../../../../../orthonormal-basis.md) for the pairing proved below is

$$
E_1=\frac i{\sqrt2}\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad
E_2=\frac1{\sqrt2}\begin{pmatrix}0&1\\-1&0\end{pmatrix},\quad
E_3=\frac i{\sqrt2}\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

Put $J_j=\sqrt2E_j$, so $J_j^2=-I$. For any unit real vector $v$, $J(v)=\sum_jv_jJ_j$ also squares to $-I$. Thus $g=\cos(\theta/2)I+\sin(\theta/2)J(v)$ belongs to $\mathrm{SU}(2)$. [Conjugation](../../../../../conjugation.md) fixes $J(v)$ and rotates its perpendicular plane by angle $\theta$ up to the orientation convention of this basis, as follows either by multiplying the displayed matrices or from their anticommutator relation $J(v)J(w)+J(w)J(v)=-2(v\cdot w)I$. Since every three-dimensional proper rotation has an axis and an angle, this proves surjectivity onto $\mathrm{SO}(3)$.

If an element is in the [kernel](../../../../../kernel-of-a-linear-map.md), it commutes with each $E_j$. Commutation with $E_3$ forces it to be diagonal; commutation with $E_1$ forces its two diagonal entries to agree. Thus it is a scalar matrix, and [determinant](../../../../../determinant.md) one and unitarity give exactly $\{I,-I\}$. Therefore **$\boxed{\mathrm{SO}(3)\cong\mathrm{SU}(2)/\{\pm I\}}$**.

The finite-dimensional complex [irreducible representations](../../../../../irreducible-representation.md) of $\mathrm{SU}(2)$ are $\operatorname{Sym}^m(\mathbb C^2)$, $m\ge0$, of dimension $m+1$. The central element $-I$ acts by $(-1)^m$, so precisely the even ones descend. **The irreducibles of $\mathrm{SO}(3)$ are $\boxed{\operatorname{Sym}^{2\ell}(\mathbb C^2),\ \ell=0,1,2,\ldots}$**, viewed as representations of the quotient, with dimensions $2\ell+1$.

## ↑ Ancestors (10)

1. [19I](../19i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
