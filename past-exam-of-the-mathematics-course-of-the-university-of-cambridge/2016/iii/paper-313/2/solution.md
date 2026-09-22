<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The real [vector space](../../../../../vector-space-split.md) of [symmetric matrices](../../../../../symmetric-matrix.md) has dimension $n(n+1)/2$. On its invertible part the derivative of the [determinant](../../../../../determinant.md) is

$$
D(\det)_B(C)=\det(B)\operatorname{tr}(B^{-1}C).
$$

At a determinant-one symmetric matrix, this derivative is nonzero: the symmetric direction $C=B$ gives value $n$. The [regular level set theorem](../../../../../regular-level-set-theorem.md) therefore yields

$$
\boxed{\dim M=\frac{n(n+1)}2-1,\qquad
T_BM=\{C=C^T:\operatorname{tr}(B^{-1}C)=0\}.}
$$

This applies to every signature component, not only positive-definite matrices.

The [special linear congruence action on symmetric matrices](../../../../../special-linear-congruence-action-on-symmetric-matrices.md) preserves symmetry because $(ABA^T)^T=ABA^T$, and preserves determinant because $\det(ABA^T)=(\det A)^2\det B=1$. The identity acts trivially and

$$
A_1\cdot(A_2\cdot B)=A_1A_2B(A_1A_2)^T=(A_1A_2)\cdot B.
$$

These verify a smooth left [Lie group action](../../../../../lie-group-action.md) of the [special linear group](../../../../../special-linear-group.md). By [Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md), it also preserves the numbers of positive and negative eigenvalues.

For $n=2$, parametrize the [symmetric matrices](../../../../../symmetric-matrix.md) by

$$
B=\begin{pmatrix}t+x&y\\y&t-x\end{pmatrix},\qquad
\det B=t^2-x^2-y^2.
$$

Thus $M$ is exactly the [two-sheeted hyperboloid](../../../../../two-sheeted-hyperboloid.md)

$$
\boxed{t^2-x^2-y^2=1,\qquad t>0\text{ or }t<0.}
$$

The two sheets consist respectively of positive-definite and negative-definite matrices. Each is preserved by the [special linear congruence action on symmetric matrices](../../../../../special-linear-congruence-action-on-symmetric-matrices.md). They are individually transitive: on the positive sheet $B=AA^T$ with $A=B^{1/2}$ and $\det A=1$; on the negative sheet use $B=-AA^T$. The stabilizer of either $I$ or $-I$ is $SO(2)$.

Differentiating the left [Lie group action](../../../../../lie-group-action.md) along $\exp(sX)$ gives the [fundamental vector field](../../../../../fundamental-vector-field.md)

$$
u_X(B)=XB+BX^T.
$$

For the three matrices in the question, their coordinate components are

$$
\begin{aligned}
u_1&=y\partial_t+y\partial_x+(t-x)\partial_y,\\
u_2&=2x\partial_t+2t\partial_x,\\
u_3&=y\partial_t-y\partial_x+(t+x)\partial_y.
\end{aligned}
$$

A sign convention matters here. With the usual [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) $[U,V]f=U(Vf)-V(Uf)$, the fundamental fields of this left action obey $[u_X,u_Y]=-u_{[X,Y]}$. Indeed, for linear coordinate fields $u_X(z)=R_Xz$, the bracket has coefficient $(R_YR_X-R_XR_Y)z$. To obtain a [Lie algebra representation](../../../../../lie-algebra-representation.md) rather than an anti-representation, use the [infinitesimal left-action sign convention](../../../../../infinitesimal-left-action-sign-convention.md)

$$
v_X(B)=\left.\frac{d}{ds}\right|_{s=0}e^{-sX}Be^{-sX^T}=-u_X(B).
$$

An explicit answer is therefore

$$
\boxed{\begin{aligned}
v_1&=-y\partial_t-y\partial_x+(x-t)\partial_y,\\
v_2&=-2x\partial_t-2t\partial_x,\\
v_3&=-y\partial_t+y\partial_x-(t+x)\partial_y.
\end{aligned}}
$$

These are tangent to the [two-sheeted hyperboloid](../../../../../two-sheeted-hyperboloid.md): applying each to $Q=t^2-x^2-y^2$ gives zero. For example,

$$
v_1(Q)=-2ty+2xy-2y(x-t)=0.
$$

They can be written on either sheet using $t=\pm\sqrt{1+x^2+y^2}$:

$$
v_1=-y\partial_x+(x-t)\partial_y,\qquad
v_2=-2t\partial_x,\qquad
v_3=y\partial_x-(t+x)\partial_y.
$$

Here the omitted $\partial_t$ component is determined by tangency, and derivatives of $t(x,y)$ must be included when computing brackets in these coordinates.

Direct matrix multiplication gives

$$
[\tau_2,\tau_1]=2\tau_1,\qquad
[\tau_2,\tau_3]=-2\tau_3,\qquad
[\tau_1,\tau_3]=\tau_2.
$$

Direct differentiation of the displayed [vector fields](../../../../../vector-field.md) gives exactly

$$
\boxed{[v_2,v_1]=2v_1,\qquad [v_2,v_3]=-2v_3,\qquad [v_1,v_3]=v_2.}
$$

For instance, in ambient $(t,x,y)$ coordinates, $[v_1,v_3]=(-2x,-2t,0)=v_2$. These are the defining relations of the [sl2 Lie algebra](../../../../../sl2-lie-algebra.md). The three fields are linearly independent over constant real coefficients: if $a v_1+b v_2+c v_3$ vanishes on a sheet, its $\partial_x$ coefficient $(-a+c)y-2bt$ forces $b=0,c=a$, and its $\partial_y$ coefficient then equals $-2at$, forcing $a=c=0$. Thus the representation is **faithful**. Their pointwise span need only have dimension two, consistent with the dimension of each sheet.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
