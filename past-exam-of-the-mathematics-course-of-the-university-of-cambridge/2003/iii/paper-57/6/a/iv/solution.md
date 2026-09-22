<h1 id="6/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $V=\mathbb R^4$ have [symplectic basis](../../../../../../../symplectic-basis.md) $(e_1,f_1,e_2,f_2)$. Fix $\mathrm{vol}=e_1\wedge f_1\wedge e_2\wedge f_2$ and define a symmetric [bilinear form](../../../../../../../bilinear-form.md) $Q$ on $\Lambda^2V$ by $u\wedge v=Q(u,v)\mathrm{vol}$. The pairings between complementary basis bivectors split this six-dimensional space into three hyperbolic planes, so $Q$ has signature $(3,3)$.

The [symplectic group](../../../../../../../symplectic-group.md) preserves volume and the bivector $\Omega=e_1\wedge f_1+e_2\wedge f_2$, obtained from the inverse symplectic form, up to its fixed sign convention. Since $Q(\Omega,\Omega)=2$, its orthogonal complement $W=\Omega^\perp$ has dimension five and signature $(2,3)$. On $W$ use $-Q$, which has signature $(3,2)$. This constructs the [exterior-square double cover of SO0(3,2)](../../../../../../../exterior-square-double-cover-of-so0-3-2.md).

If an element acts trivially on $W$, it also fixes $\Omega$, so its action on the entire [exterior square](../../../../../../../exterior-square.md) is the identity. Every decomposable bivector then shows that its two-plane is preserved. A line is the intersection of two such planes; hence every line is preserved, and the matrix is scalar. Its exterior-square action forces its scalar square to equal one, giving precisely $\pm I$.

The derivative is injective by the same infinitesimal argument: zero action on $\Lambda^2V$ forces an infinitesimal scalar, whose induced scalar there is twice its value and therefore zero. The [symplectic Lie algebra](../../../../../../../symplectic-lie-algebra.md) has dimension $2^2+2(2\cdot3/2)=10$, from blocks $\left(\begin{smallmatrix}A&B\\C&-A^T\end{smallmatrix}\right)$ with symmetric $B,C$. The orthogonal Lie algebra in five dimensions also has dimension ten. Thus the image is open. Real symplectic polar decomposition has connected compact factor $U(2)$ and a contractible positive symplectic factor, so $Sp(4,\mathbb R)$ is connected and its image is exactly the identity component:

$$
\boxed{Sp(4,\mathbb R)/\{\pm I\}\cong SO_0(3,2).}
$$

As in the preceding noncompact cases, this does not identify the quotient with the disconnected full $SO(3,2)$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
