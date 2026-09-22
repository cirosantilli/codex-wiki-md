<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the normalization in which a [Hodge metric](../../../../../hodge-metric.md) is a [Kähler metric](../../../../../kahler-metric.md) whose [Kähler form](../../../../../kahler-form.md) $\omega$ represents the image of an [integral cohomology](../../../../../integral-cohomology.md) class in real [de Rham cohomology](../../../../../de-rham-cohomology.md). Equivalently, all its periods on integral two-cycles are integers. A convention using $\omega/(2\pi)$ only rescales the metric and does not change existence. An invariant metric on a [complex torus](../../../../../complex-torus.md) is one preserved by every translation; its pullback to $\mathbb C^n$ has constant coefficients.

Let $T=\mathbb C^n/\Lambda$ carry a [Hodge metric](../../../../../hodge-metric.md). Average its [Kähler form](../../../../../kahler-form.md) over translations using normalized [Haar measure](../../../../../haar-measure.md):

$$
\omega_0=\int_T t_a^*\omega\,da.
$$

This [averaging Kähler forms over a complex torus](../../../../../averaging-kahler-forms-over-a-complex-torus.md) preserves reality, type $(1,1)$, closedness and positivity. Indeed, for any nonzero tangent vector, the quantity being averaged in $\omega(v,Jv)$ is strictly positive. Every translation is homotopic to the identity, since a path from $0$ to $a$ supplies such a homotopy. Thus $[\omega_0]=[\omega]$, as is seen either on [de Rham cohomology](../../../../../de-rham-cohomology.md) or by integrating over two-cycles. The average is translation invariant by invariance of [Haar measure](../../../../../haar-measure.md) and determines a [Kähler metric](../../../../../kahler-metric.md) $g_0(v,w)=\omega_0(v,Jw)$. Its class is still integral. The reverse implication is immediate. Therefore **a Hodge metric exists exactly when an invariant one does**.

Here is the [Riemann bilinear criterion for a period matrix](../../../../../riemann-bilinear-criterion-for-a-period-matrix.md), with the signs kept explicit. For the [period matrix of a complex torus](../../../../../period-matrix-of-a-complex-torus.md), use real coordinates $t_1,\ldots,t_{2n}$ along the lattice basis, so $z=\Omega t$. An invariant real two-form is

$$
\omega=\frac12\sum_{i,j}Q_{ij}\,dt_i\wedge dt_j,\qquad Q^t=-Q.
$$

Its period on the coordinate two-torus $(i,j)$ is $Q_{ij}$; these tori generate integral second homology. Thus integrality of the class is exactly $Q\in M_{2n}(\mathbb Z)$. Positivity of a [Kähler form](../../../../../kahler-form.md) makes $Q$ nonsingular. Because the lattice basis is a real basis of $\mathbb C^n$, the complex matrix

$$
T_0=\begin{pmatrix}\Omega\\\bar\Omega\end{pmatrix}
$$

is invertible: its rows recover the real and imaginary parts of the coordinates. In the coordinates $(z,\bar z)$, the matrix of the two-form is $T_0^{-t}QT_0^{-1}$, whose inverse is $T_0Q^{-1}T_0^t$.

The [differential form of type (p, q)](../../../../../differential-form-of-type-p-q.md) condition $(1,1)$ says that the two diagonal blocks of the form matrix vanish. Since the form is nonsingular, this is equivalent to the diagonal blocks of its inverse vanishing. Because $Q$ is real, these inverse blocks vanish exactly when

$$
\Omega Q^{-1}\Omega^t=0.
$$

Set $H=-i\Omega Q^{-1}\bar\Omega^t$. Skew-symmetry and reality of $Q$ give $H^*=H$, and the full inverse matrix is

$$
T_0Q^{-1}T_0^t=
\begin{pmatrix}0&iH\\-iH^t&0\end{pmatrix}.
$$

Inverting these blocks identifies the two-form explicitly:

$$
\omega=i\sum_{a,b}(H^{-1})_{ba}\,dz_a\wedge d\bar z_b.
$$

For a vector with complex coordinate column $v$, evaluation yields $\omega(v,Jv)=2v^*H^{-1}v$. Hence this two-form is positive exactly when $H$ is a [Hermitian positive-definite matrix](../../../../../hermitian-positive-definite-matrix.md). This proves both directions: an invariant [Hodge metric](../../../../../hodge-metric.md) gives such an integral $Q$, and any such $Q$ produces a constant positive real closed $(1,1)$-form of integral periods. In particular,

$$
\boxed{T\text{ admits a Hodge metric}\iff
\exists Q\in M_{2n}(\mathbb Z),\
Q^t=-Q,\ \det Q\ne0,\
\Omega Q^{-1}\Omega^t=0,\
-i\Omega Q^{-1}\bar\Omega^t>0.}
$$

As a sign check, for $\Omega=(I,iI)$ and $Q=\begin{pmatrix}0&I\\-I&0\end{pmatrix}$ the last matrix is $2I$, and the associated form is $(i/2)\sum dz_a\wedge d\bar z_a$.

For the specified two-dimensional [complex torus](../../../../../complex-torus.md), put

$$
J=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad
s=\sqrt2,\qquad A=I+sJ.
$$

The real and imaginary period vectors are independent because $\det A=3$, so they do form a full lattice. Suppose a polarization matrix $Q$ existed. Its inverse $R=Q^{-1}$ is a rational skew-symmetric matrix, and hence has the block expression

$$
R=\begin{pmatrix}aJ&B\\-B^t&cJ\end{pmatrix},
\qquad a,c\in\mathbb Q,\quad B\in M_2(\mathbb Q).
$$

The first condition of the [Riemann bilinear criterion for a period matrix](../../../../../riemann-bilinear-criterion-for-a-period-matrix.md) becomes

$$
0=\Omega R\Omega^t=(a-3c)J+i(BA^t-AB^t).
$$

Separating real and imaginary parts gives $a=3c$ and

$$
B-B^t=s(BJ+JB^t).
$$

The matrices on both sides have rational entries except for the factor $\sqrt2$. Irrationality of $\sqrt2$ therefore implies $B=B^t$ and $BJ+JB=0$. For a symmetric two-by-two matrix the latter expression is $(\operatorname{Tr}B)J$, so $\operatorname{Tr}B=0$. The candidate [Hermitian matrix](../../../../../hermitian-operator.md) is now

$$
H=-i\Omega R\bar\Omega^t
=AB+BA^t-6icJ.
$$

Since $A=I+sJ$, $B$ is symmetric and traceless, and $J$ is skew-symmetric, $\operatorname{Tr}(AB+BA^t)=2\operatorname{Tr}B=0$ and $\operatorname{Tr}J=0$. Thus $\operatorname{Tr}H=0$. A [Hermitian positive-definite matrix](../../../../../hermitian-positive-definite-matrix.md) has strictly positive [eigenvalues](../../../../../eigenvalue.md), hence strictly positive [trace](../../../../../matrix-trace.md). This contradiction proves

$$
\boxed{\mathbb C^2/\Lambda\text{ admits no Hodge metric}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
