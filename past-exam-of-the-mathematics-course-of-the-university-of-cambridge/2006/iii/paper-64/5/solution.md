<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The two unheaded requests are addressed here; the individual group-cover calculations are in the scoped parts below. A [quaternion](../../../../../quaternion.md) $q=a+bi+cj+dk$ has [norm](../../../../../norm.md) $|q|^2=a^2+b^2+c^2+d^2$. Thus the [unit quaternions](../../../../../unit-quaternion.md) form exactly the sphere $S^3\subset\mathbb R^4$, with [quaternion](../../../../../quaternion.md) multiplication giving its smooth group structure. The explicit identification with the [special unitary group](../../../../../special-unitary-group.md) $SU(2)$ is

$$
q\longmapsto
\begin{pmatrix}
a+ib&c+id\\
-c+id&a-ib
\end{pmatrix}.
$$

The [matrices](../../../../../matrix.md) representing $i,j,k$ satisfy the [quaternion](../../../../../quaternion.md) multiplication relations. The displayed [matrix](../../../../../matrix.md) obeys $U^\dagger U=|q|^2I$ and $\det U=|q|^2$; conversely every $SU(2)$ [matrix](../../../../../matrix.md) has that form with $|q|=1$. Hence **$S^3$ is the manifold of [unit quaternions](../../../../../unit-quaternion.md), and its group is $SU(2)$**.

For the [exterior-square double cover of SO(3,3)](../../../../../exterior-square-double-cover-of-so-3-3.md), fix a [basis](../../../../../basis.md) $e_1,\ldots,e_4$ and volume element $v=e_1\wedge e_2\wedge e_3\wedge e_4$. Define the symmetric bilinear form $Q$ on the six-dimensional exterior square by

$$
\alpha\wedge\beta=Q(\alpha,\beta)v.
$$

It is symmetric because [two-forms](../../../../../2-form.md) commute under the [wedge product](../../../../../exterior-product.md). Put

$$
a_1=e_1\wedge e_2,\quad a_2=e_1\wedge e_3,\quad a_3=e_1\wedge e_4,\qquad
b_1=e_3\wedge e_4,\quad b_2=-e_2\wedge e_4,\quad b_3=e_2\wedge e_3.
$$

Then $Q(a_i,a_j)=Q(b_i,b_j)=0$ and $Q(a_i,b_j)=\delta_{ij}$. The Gram [matrix](../../../../../matrix.md) is $\begin{pmatrix}0&I_3\\I_3&0\end{pmatrix}$: the vectors $(a_i+b_i)/\sqrt2$ have [norm](../../../../../norm.md) $+1$, while $(a_i-b_i)/\sqrt2$ have [norm](../../../../../norm.md) $-1$. Therefore **the quadratic form $\omega\mapsto\omega\wedge\omega$ has signature $(3,3)$**.

For $A\in SL(4,\mathbb R)$,

$$
(\Lambda^2A\,\alpha)\wedge(\Lambda^2A\,\beta)
=\Lambda^4A(\alpha\wedge\beta)=\alpha\wedge\beta.
$$

Thus $\rho(A)=\Lambda^2A$ preserves $Q$. The [special linear group](../../../../../special-linear-group.md) is connected: [polar decomposition of an invertible real matrix](../../../../../polar-decomposition-of-an-invertible-real-matrix.md) writes $A=OP$ with $O\in SO(4)$ and $P$ positive definite of [determinant](../../../../../determinant.md) one, and both factors can be joined to the identity. The image consequently lies in $SO_0(3,3)$.

If $\Lambda^2A=I$, then $Au\wedge Aw=u\wedge w$ for every pair, so $A$ preserves every two-plane. A line is an intersection of two such planes, hence every line is preserved. A [linear map](../../../../../linear-map.md) preserving every line is scalar: apply it to [basis](../../../../../basis.md) vectors and then to their pairwise sums. Thus $A=\lambda I$, and $\Lambda^2A=I$ forces $\lambda^2=1$. The kernel is exactly $\{\pm I\}$. It is discrete, so the derivative of $\rho$ is injective. Both [Lie algebras](../../../../../lie-algebra-split.md) have dimension $15$, making the image open; an open subgroup of a connected group is the whole group. Hence

$$
\boxed{SO_0(3,3)\cong SL(4,\mathbb R)/\{\pm I\}.}
$$

The identity-component restriction is essential. The same principle of an explicit form-preserving representation, kernel calculation and dimension argument supplies the five remaining covers.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
