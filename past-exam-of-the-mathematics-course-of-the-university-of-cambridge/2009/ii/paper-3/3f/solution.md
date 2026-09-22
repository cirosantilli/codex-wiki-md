<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Consider the [Möbius transformations](../../../../../mobius-transformation.md)

$$
A(z)=z+2,\qquad B(z)=\frac{z}{2z+1},\qquad
A=\begin{pmatrix}1&2\\0&1\end{pmatrix},\quad B=\begin{pmatrix}1&0\\2&1\end{pmatrix}.
$$

Their [group](../../../../../group-split.md) lies in $\operatorname{PSL}_2(\mathbb Z)$, which is a [discrete subgroup](../../../../../discrete-subgroup.md) of the [Möbius group](../../../../../mobius-group.md): integer entries cannot approach the identity matrix except by eventually equalling it, and passing to the quotient by $\{I,-I\}$ preserves this property.

For freeness let $X=\{x\in\mathbb R:|x|>1\}$ and $Y=\{x\in\mathbb R:|x|<1\}$. For every nonzero integer $n$, $A^n(Y)=(2n-1,2n+1)\subset X$ and

$$
B^n(x)=\frac{x}{2nx+1},\qquad |B^n(x)|=\frac1{|2n+1/x|}<1\quad(x\in X).
$$

A reduced word involving both generators can be conjugated to a cyclically reduced word beginning with $A^n$ and ending with a nonzero power of $B$, after interchanging the generators if necessary. Repeated use of these inclusions shows that this word sends $X$ into the proper subset $A^n(Y)$ of $X$, so it cannot be the identity. Nonzero pure powers of either generator are also nonidentity. This is the [ping-pong lemma](../../../../../ping-pong-lemma.md) in this particular action, and proves that $\boxed{\langle A,B\rangle\cong F_2}$ is a [free group](../../../../../free-group.md) of rank two as well as a [discrete subgroup](../../../../../discrete-subgroup.md) of $\operatorname{PSL}_2(\mathbb C)$.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
