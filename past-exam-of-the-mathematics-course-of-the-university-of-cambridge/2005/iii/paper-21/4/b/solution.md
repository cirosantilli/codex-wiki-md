<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In weight one, the [Hodge numbers](../../../../../../hodge-number.md) are $h^{1,0}=h^{0,1}=r$, and the [Hodge filtration](../../../../../../hodge-filtration.md) is determined by the $r$-plane $H=F^1$. The bilinear orthogonality condition is $\psi(H,H)=0$. An isotropic $r$-plane in a symplectic $2r$-space is a [Lagrangian subspace](../../../../../../lagrangian-subspace.md), so

$$
\boxed{\check D=\operatorname{SpGr}(r,2r)
=\operatorname{LGr}(\mathbb C^{2r},\psi).}
$$

The ordinary [Grassmannian](../../../../../../grassmannian.md) has dimension $r^2$. Restriction of the alternating form to an $r$-plane imposes $r(r-1)/2$ independent conditions. Equivalently, near a fixed Lagrangian plane, transverse Lagrangians are graphs of [symmetric matrices](../../../../../../symmetric-matrix.md), with $r(r+1)/2$ independent entries. Therefore

$$
\boxed{\dim_{\mathbb C}\check D=\frac{r(r+1)}2.}
$$

Write $\mathbb C^{2r}=\mathbb C^r\oplus\mathbb C^r$ in the block order of the given matrix. On $D$, positivity is $i\psi(v,\bar v)>0$ for every nonzero $v\in H$. The plane $H$ cannot contain $(x,0)\ne0$, because that vector has $\psi(v,\bar v)=0$. Projection onto the second coordinate factor is therefore [injective](../../../../../../injective-function.md) on $H$ and, by equal dimensions, an [isomorphism](../../../../../../isomorphism.md). There is a unique matrix $Z$ such that

$$
H=H_Z=\{(Zu,u):u\in\mathbb C^r\}.
$$

For $v=(Zu,u)$ and $v'=(Zw,w)$, direct evaluation gives

$$
\psi(v,v')=u^{\mathsf T}(Z-Z^{\mathsf T})w.
$$

Thus isotropy is exactly $Z=Z^{\mathsf T}$. For such $Z$,

$$
i\psi(v,\bar v)
=i\,u^{\mathsf T}(\bar Z-Z)\bar u
=2u^{\mathsf T}(\operatorname{Im}Z)\bar u.
$$

Hence positivity is precisely [positive definiteness](../../../../../../positive-definiteness.md) of $\operatorname{Im}Z$. Conversely, symmetry and this inequality define a positive Lagrangian plane; it is opposed to its conjugate because $(Z-\bar Z)u=0$ forces $u=0$. We have explicitly identified

$$
\boxed{D\cong\mathfrak H_r=
\{Z\in M_r(\mathbb C):Z=Z^{\mathsf T},\
\operatorname{Im}Z>0\},}
$$

the [Siegel upper half-space](../../../../../../siegel-upper-half-space.md). The choice of the graph $(Zu,u)$, rather than $(u,Zu)$, is what matches the sign of the given [symplectic form](../../../../../../symplectic-form.md).

Let an integral element of the [symplectic group](../../../../../../symplectic-group.md) have block matrix

$$
g=\begin{pmatrix}A&B\\ C&D_0\end{pmatrix}.
$$

Acting on graph vectors gives

$$
g(Zu,u)=((AZ+B)u,(CZ+D_0)u).
$$

The image remains a positive Lagrangian plane, so its second projection is invertible. Thus $CZ+D_0$ is invertible and the induced action is

$$
\boxed{g\cdot Z=(AZ+B)(CZ+D_0)^{-1}.}
$$

The symplectic identities give symmetry of this matrix, and preservation of $i\psi(v,\bar v)$ gives

$$
\operatorname{Im}(g\cdot Z)
=(C\bar Z+D_0)^{-\mathsf T}
(\operatorname{Im}Z)(CZ+D_0)^{-1}>0.
$$

This is a Hermitian congruence by an invertible matrix, so it proves preservation of the positive domain as well as describing the action. These are coordinates on marked [Hodge structures](../../../../../../hodge-structure.md); passing to the integral-group quotient forgets the symplectic marking.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
