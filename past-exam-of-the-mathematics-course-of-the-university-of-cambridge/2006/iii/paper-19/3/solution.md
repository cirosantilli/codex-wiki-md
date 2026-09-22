<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $v=(v_1,v_2,v_3)$ define the [skew-symmetric matrix](../../../../../skew-symmetric-matrix.md)

$$
\widehat v=\begin{pmatrix}0&-v_3&v_2\\v_3&0&-v_1\\-v_2&v_1&0\end{pmatrix}.
$$

Then $\widehat v x=v\times x$. This is a [linear isomorphism](../../../../../linear-isomorphism.md) $\mathbb R^3\to\mathfrak{so}(3)$, with inverse $\phi(\xi)=(\xi_{32},\xi_{13},\xi_{21})$. Since rotations preserve the [cross product](../../../../../cross-product.md),

$$
R\widehat vR^{-1}=\widehat{Rv}\qquad(R\in SO(3)).
$$

Thus $\phi$ intertwines the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) with the standard [representation](../../../../../group-representation.md). The vector triple-product identity gives, for every $x$,

$$
[\widehat v,\widehat w]x=v\times(w\times x)-w\times(v\times x)=(v\times w)\times x.
$$

Consequently $[\widehat v,\widehat w]=\widehat{v\times w}$ and the chosen normalization satisfies

$$
\boxed{\phi([\xi,\eta])=\phi(\xi)\times\phi(\eta).}
$$

No undetermined scale remains in this explicit [matrix](../../../../../matrix.md) convention.

Identify $SU(2)$ with the [unit quaternions](../../../../../unit-quaternion.md) using

$$
q=z+w j\longmapsto\begin{pmatrix}z&w\\-\overline w&\overline z\end{pmatrix},\qquad |z|^2+|w|^2=1.
$$

The relations $jz=\overline z j$ and $j^2=-1$ verify multiplication, and every [matrix](../../../../../matrix.md) in $SU(2)$ has this form. If $v$ is imaginary, then $\overline v=-v$. Quaternionic [conjugation](../../../../../conjugation.md) reverses [product order](../../../../../product-order.md) and $q^{-1}=\overline q$, so

$$
\overline{qvq^{-1}}=q\overline v q^{-1}=-qvq^{-1}.
$$

Thus [conjugation](../../../../../conjugation.md) preserves $\operatorname{Im}\mathbb H\cong\mathbb R^3$. Multiplicativity of the [quaternion](../../../../../quaternion.md) norm shows that this action preserves the [inner product](../../../../../inner-product.md). The [unit quaternions](../../../../../unit-quaternion.md) form the [connected](../../../../../connected-space.md) three-sphere, so its [determinant](../../../../../determinant.md), equal to one at the identity, is always one. We obtain a homomorphism $C:SU(2)\to SO(3)$.

Its [group kernel](../../../../../kernel-of-a-group-homomorphism.md) consists of [unit quaternions](../../../../../unit-quaternion.md) commuting with every imaginary [quaternion](../../../../../quaternion.md). Commuting with both $i$ and $j$ forces a [quaternion](../../../../../quaternion.md) to be real, so the [group kernel](../../../../../kernel-of-a-group-homomorphism.md) is exactly $\{\pm1\}$. To prove [surjectivity](../../../../../surjective-function.md) explicitly, let $u$ be a unit imaginary [quaternion](../../../../../quaternion.md) and put $q=\cos(\theta/2)+u\sin(\theta/2)$. For imaginary $u,v$, multiplication satisfies $uv=-u\cdot v+u\times v$. Expanding $qvq^{-1}$ therefore gives

$$
qvq^{-1}=v\cos\theta+(u\times v)\sin\theta+u(u\cdot v)(1-\cos\theta).
$$

This is the [Rodrigues rotation formula](../../../../../rodrigues-rotation-formula.md) about axis $u$. Every element of $SO(3)$ has such an axis-angle description: an odd-dimensional [orthogonal matrix](../../../../../orthogonal-matrix.md) of [determinant](../../../../../determinant.md) one has an eigenvector of [eigenvalue](../../../../../eigenvalue.md) one, and its action on the perpendicular plane is a plane rotation. Hence $C$ is onto, and

$$
\boxed{SU(2)/\{\pm I_2\}\cong SO(3).}
$$

This is the quaternionic form of the [Adjoint double cover from SU(2) to SO(3)](../../../../../adjoint-double-cover-from-su-2-to-so-3.md). Its differential sends an imaginary [quaternion](../../../../../quaternion.md) $u$ to $2\widehat u$, because $[u,v]=2u\times v$, consistent with the bracket normalization used above.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
