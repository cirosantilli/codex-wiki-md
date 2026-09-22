<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

By the [spectral theorem](../../../spectral-theorem.md) a [symmetric positive-definite matrix](../../../symmetric-positive-definite-matrix.md) $C$ has $C=Q\operatorname{diag}(c_i)Q^{\mathsf T}$, with $Q$ [orthogonal](../../../orthogonal-vectors.md) and $c_i>0$. Define $S=Q\operatorname{diag}(\sqrt{c_i})Q^{\mathsf T}$. It is [symmetric](../../../symmetric-relation.md) [positive-definite](../../../positive-definite-bilinear-form.md) and $S^2=C$. For [uniqueness](../../../uniqueness.md), any [symmetric](../../../symmetric-relation.md) [positive-definite](../../../positive-definite-bilinear-form.md) square root $T$ commutes with $C=T^2$, hence preserves each [eigenspace](../../../eigenspace.md) of $C$. On its $c$-[eigenspace](../../../eigenspace.md), $T$ is [symmetric](../../../symmetric-relation.md) [positive-definite](../../../positive-definite-bilinear-form.md) and all its [eigenvalues](../../../eigenvalue.md) have square $c$, so all equal $\sqrt c$. Therefore $T=S$, including repeated [eigenspaces](../../../eigenspace.md).

For $\det F>0$, put

$$
\boxed{U=(F^{\mathsf T}F)^{1/2},\quad R=FU^{-1},\quad V=RUR^{\mathsf T}=(FF^{\mathsf T})^{1/2}.}
$$

Then $R^{\mathsf T}R=I$ and $\det R=\det F/\det U>0$, so $R\in SO(3)$; also $F=RU=VR$. Any other [right polar decomposition](../../../polar-decomposition-in-continuum-mechanics.md) has $F^{\mathsf T}F=U^2$, so [uniqueness](../../../uniqueness.md) of the positive root fixes $U$ and then $R$. The left factor is consequently fixed too.

The principal stretches $v_i$ are the positive [eigenvalues](../../../eigenvalue.md) of $U$, equivalently the [singular values](../../../singular-value.md) of $F$. For a [unit vector](../../../unit-vector.md) $N=\sum_i c_iN_i$ in an orthonormal [eigenbasis](../../../eigenbasis.md) of $U$,

$$
|FN|^2=N^{\mathsf T}U^2N=\sum_i v_i^2c_i^2\leq v_{\max}^2\sum_i c_i^2=v_{\max}^2.
$$

Thus $\boxed{\max_{|N|=1}|FN|=v_{\max}}$, attained precisely by the [unit vectors](../../../unit-vector.md) in the [eigenspace](../../../eigenspace.md) of $U$ belonging to $v_{\max}$. With a simple largest [eigenvalue](../../../eigenvalue.md) these are its two opposite unit [eigenvectors](../../../eigenvector.md); degeneracy allows every unit combination within that [eigenspace](../../../eigenspace.md).

For the [simple shear](../../../simple-shear.md),

$$
F=\begin{pmatrix}1&\gamma&0\\0&1&0\\0&0&1\end{pmatrix},\qquad C=F^{\mathsf T}F=\begin{pmatrix}1&\gamma&0\\\gamma&1+\gamma^2&0\\0&0&1\end{pmatrix}.
$$

A line with nonzero direction $N$ keeps its length exactly when

$$
|FN|^2-|N|^2=\gamma N_2(2N_1+\gamma N_2)=0.
$$

Hence $\boxed{N_2=0\quad\text{or}\quad2N_1+\gamma N_2=0}$, with $N_3$ arbitrary. Every segment in the cube [parallel](../../../linear-dependence.md) to one of these directions preserves length; there is no restriction on its starting point other than remaining in the cube.

The two in-[plane](../../../plane.md) stretches are $v_\pm=(\sqrt{4+\gamma^2}\pm\gamma)/2$, and the third is one. A maximizing direction for $\gamma>0$ is $N\parallel(1,v_+,0)$, since the $C$ [eigenvalue](../../../eigenvalue.md) equation gives $N_2/N_1=(v_+^2-1)/\gamma=v_+$. Therefore $\boxed{N\to\pm(1,1,0)/\sqrt2}$ as $\gamma\downarrow0$. At exactly zero shear all directions tie; the limit refers to the selected maximizing direction for positive shear. These are the [length-preserving directions and principal directions of simple shear](../../../length-preserving-directions-and-principal-directions-of-simple-shear.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2008](../../2008-split.md)
3. [Past exam of the solid mechanics course of the University of Oxford](../../split.md)
4. [Solid mechanics course of the University of Oxford](../../../solid-mechanics-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
