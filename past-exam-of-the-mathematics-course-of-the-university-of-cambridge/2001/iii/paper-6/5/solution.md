<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [bounded linear operator](../../../../../continuous-linear-operator.md) $T:E\to F$, write the weak square norm of a finite family as

$$
w_2(x_1,\ldots,x_m)=\sup_{\phi\in E^*,\ \|\phi\|\le1}\left(\sum_{j=1}^m|\phi(x_j)|^2\right)^{1/2}.
$$

It is a [2-summing operator](../../../../../2-summing-operator.md) if $(\sum_j\|Tx_j\|^2)^{1/2}\le Cw_2(x_1,\ldots,x_m)$ for all finite families, and $\pi_2(T)$ is the least such $C$. This specializes the definition of an [absolutely p-summing operator](../../../../../absolutely-p-summing-operator.md).

First let $E=H_1$, $F=H_2$ be [Hilbert spaces](../../../../../hilbert-space-split.md). For the column operator $A:\ell_2^m\to H_1$, $Ae_j=x_j$, the [Riesz representation theorem](../../../../../riesz-representation-theorem.md) gives $w_2(x_1,\ldots,x_m)=\|A^*\|=\|A\|$. If $T$ is a [Hilbert-Schmidt operator](../../../../../hilbert-schmidt-operator.md), the [Parseval identity](../../../../../parseval-identity.md) applied to orthonormal bases gives

$$
\sum_{j=1}^m\|Tx_j\|^2=\|TA\|_{\mathrm{HS}}^2
=\sum_\alpha\|A^*T^*f_\alpha\|^2
\le\|A\|^2\sum_\alpha\|T^*f_\alpha\|^2
=\|A\|^2\|T\|_{\mathrm{HS}}^2.
$$

Thus $\pi_2(T)\le\|T\|_{\mathrm{HS}}$. Conversely test the summing inequality on any finite orthonormal family in $H_1$. Its weak square norm is $1$, by the [Bessel inequality](../../../../../bessel-s-inequality.md), with equality by choosing one of its vectors. Hence $\sum_j\|Te_j\|^2\le\pi_2(T)^2$. Taking the supremum over finite subsets of an [orthonormal basis](../../../../../orthonormal-basis.md) proves the [Hilbert-Schmidt operator](../../../../../hilbert-schmidt-operator.md) condition and the reverse norm inequality. These basis sums work even for nonseparable [Hilbert spaces](../../../../../hilbert-space-split.md), being understood as suprema of finite subsums. Therefore

$$
\boxed{T\text{ is Hilbert-Schmidt}\iff T\text{ is 2-summing},\qquad \pi_2(T)=\|T\|_{\mathrm{HS}}.}
$$

For an $n$-dimensional [normed vector space](../../../../../normed-vector-space.md) $E$, again associate a family $(x_j)$ with $A:\ell_2^m\to E$. By the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) and scalar Euclidean duality,

$$
\|A\|=\sup_{\|\phi\|\le1}\left(\sum_j|\phi(x_j)|^2\right)^{1/2}=w_2(x_1,\ldots,x_m).
$$

Let $Q$ be the [orthogonal projection](../../../../../orthogonal-projection.md) onto $(\ker A)^\perp$, whose dimension is at most $n$. Since $A=AQ$, the [trace](../../../../../matrix-trace.md) of $Q$ gives

$$
\sum_j\|x_j\|_E^2\le\|A\|^2\sum_j\|Qe_j\|_2^2
=\|A\|^2\operatorname{rank}A\le n\,w_2(x_1,\ldots,x_m)^2.
$$

This proves $\pi_2(I_E)\le\sqrt n$ for every norm, without comparing that norm to an arbitrary Euclidean norm.

To obtain equality and the projection bound, choose a maximum-volume centered [ellipsoid](../../../../../ellipsoid.md) inside the unit ball $B_E$ and use coordinates in which it is the Euclidean ball $B_2$. In the real case this is the [John ellipsoid](../../../../../john-ellipsoid.md); in the complex case maximize among Hermitian ellipsoids. There are unit contact vectors $u_r\in\partial B_E\cap\partial B_2$ and positive weights $c_r$ with the [John contact decomposition](../../../../../john-contact-decomposition.md)

$$
\sum_r c_r u_ru_r^*=I_E,\qquad \sum_r c_r=n.
$$

For completeness, the maximum-volume argument gives this identity. If $I_E$ were outside the closed convex cone of the contact matrices, finite-dimensional separation would supply a symmetric, or Hermitian, matrix $D$ with $\operatorname{tr}D>0$ and $u^*Du\le0$ at every contact. The cone is closed because its compact generators have trace one. Subtract a sufficiently small multiple of the identity to make all contact inequalities strict while retaining positive trace. The support function of $(I+tD)B_2$ decreases near the contact directions for small $t>0$; away from them the strict gap between the support functions of $B_E$ and $B_2$ permits the same small deformation. Thus this deformed ball still lies in $B_E$. Its volume increases, since the real determinant is $1+t\operatorname{tr}D+O(t^2)$ in the real case and $|\det_{\mathbb C}(I+tD)|^2=1+2t\operatorname{tr}D+O(t^2)$ in the complex case. This contradicts maximality. The finite-dimensional convex-cone representation gives finitely many contacts, and taking traces gives the sum of the weights.

At a contact $u_r$, a supporting hyperplane to $B_E$ also supports $B_2$. The Euclidean ball has a unique supporting direction there, so the corresponding functional is $\phi_r(x)=u_r^*x$ and has dual norm one on $E$. In the complex case balancedness of $B_E$ turns the real support bound into $|\phi_r(x)|\le\|x\|_E$. Also $B_2\subseteq B_E$ gives $\|x\|_E\le|x|_2$. For any dual-unit functional $\phi$, this containment implies that its Euclidean norm is at most one. Apply the summing definition to $x_r=\sqrt{c_r}\,u_r$:

$$
\sum_r\|x_r\|_E^2=\sum_r c_r=n,\qquad
\sum_r|\phi(x_r)|^2=|\phi|_2^2\le1.
$$

The weak square norm is exactly one, since any contact functional attains that Euclidean norm. Hence $\pi_2(I_E)\ge\sqrt n$. Together with the upper estimate, **the norm is**

$$
\boxed{\pi_2(I_E)=\sqrt n.}
$$

This proves the [2-summing norm of a finite-dimensional identity](../../../../../2-summing-norm-of-a-finite-dimensional-identity.md) formula.

Finally retain the preceding finite-dimensional hypothesis when $E\subseteq X$. Extend each $\phi_r$ to a dual-unit functional $\widetilde\phi_r$ on $X$ using the real or complex [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). Define

$$
P:X\to E,\qquad Px=\sum_r c_r\widetilde\phi_r(x)u_r.
$$

The contact identity gives $P|_E=I_E$, hence $P^2=P$ and its range is $E$. The synthesis operator $(a_r)\mapsto\sum_r\sqrt{c_r}a_ru_r$ has Euclidean operator norm one, because its product with its adjoint is the identity. Therefore

$$
\|Px\|_E\le|Px|_2\le\left(\sum_r c_r|\widetilde\phi_r(x)|^2\right)^{1/2}
\le\sqrt{\sum_r c_r}\,\|x\|_X=\sqrt n\,\|x\|_X.
$$

Thus **the [linear projection](../../../../../projection-linear-algebra.md) satisfies $\boxed{\|P\|\le\sqrt n}$**, the [Kadec-Snobar projection bound](../../../../../kadec-snobar-projection-bound.md). If $n=0$, the zero projection gives the same conclusion. No assertion about arbitrary infinite-dimensional subspaces is required.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
