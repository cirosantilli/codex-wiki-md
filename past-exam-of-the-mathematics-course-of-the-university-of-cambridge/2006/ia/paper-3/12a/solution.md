<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

A Cartesian [isotropic tensor](../../../../../isotropic-tensor.md) is unchanged by every proper [rotation matrix](../../../../../rotation-matrix.md). For a rank-two tensor this means $B'=RBR^{\mathsf T}=B$, or $B'_{ij}=R_{ik}R_{jl}B_{kl}=B_{ij}$. No symmetry of $B$ is assumed. For a quarter-turn about the $z$ axis,

$$
R_z=\begin{pmatrix}0&-1&0\\1&0&0\\0&0&1\end{pmatrix},\qquad
R_zBR_z^{\mathsf T}=\begin{pmatrix}
B_{22}&-B_{21}&-B_{23}\\
-B_{12}&B_{11}&B_{13}\\
-B_{32}&B_{31}&B_{33}
\end{pmatrix}.
$$

Comparing entries yields $B_{11}=B_{22}$, $B_{12}=-B_{21}$, $B_{13}=-B_{23}= -B_{13}$, and $B_{31}=-B_{32}=-B_{31}$. In particular,

$$
\boxed{B_{13}=B_{31}=B_{23}=B_{32}=0}.
$$

The remaining matrix has the form $\begin{pmatrix}b&c&0\\-c&b&0\\0&0&d\end{pmatrix}$. A quarter-turn about the $x$ axis gives

$$
R_x=\begin{pmatrix}1&0&0\\0&0&-1\\0&1&0\end{pmatrix},\qquad
R_xBR_x^{\mathsf T}=\begin{pmatrix}b&0&c\\0&d&0\\-c&0&b\end{pmatrix}.
$$

Invariance now forces $c=0$ and $d=b$, proving that an [isotropic second-rank tensor](../../../../../isotropic-second-rank-tensor.md) is

$$
\boxed{B_{ij}=b\delta_{ij}},
$$

a scalar multiple of the [Kronecker delta](../../../../../kronecker-delta.md).

For the final unheaded conductivity identity, let $P=nn^{\mathsf T}$, the orthogonal [projection](../../../../../projection-linear-algebra.md) onto the unit vector $n$. Then $P^2=P$ and the [uniaxial conductivity tensor](../../../../../uniaxial-conductivity-tensor.md) is $\sigma=\alpha I+\gamma P$. The antisymmetric tensor $D$ sends a vector $v$ to $v\times n$. Applying it twice and using the vector triple product gives

$$
D^2v=(v\times n)\times n=n(n\cdot v)-v,
\qquad D^2=P-I.
$$

Consequently

$$
\sigma D^2=(\alpha I+\gamma P)(P-I)=\alpha P-\alpha I.
$$

This equals $-\sigma=-\alpha I-\gamma P$ exactly when $(\alpha+\gamma)P=0$. Since $P$ has rank one and is nonzero, the requested parameter is

$$
\boxed{\gamma=-\alpha}.
$$

At this value conductivity vanishes along $n$; it is precisely the singular case excluded in part (ii), so there is no conflict with that part's conclusion.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
