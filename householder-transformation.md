# Householder transformation

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Householder_transformation)

A [Householder transformation](householder-transformation.md) is a [reflection](reflection-mathematics.md) that leaves every direction in a chosen [hyperplane](hyperplane.md) fixed and reverses its normal direction. For a real [unit vector](unit-vector.md) $u$, its [matrix](matrix.md) is

$$
\boxed{H=I-2uu^T.}
$$

To understand the formula, decompose any [vector](vector.md) into its [orthogonal projection](orthogonal-projection.md) onto the normal and a perpendicular component:

$$
x=x_\parallel+x_\perp,\qquad
x_\parallel=(u^Tx)u,\qquad u^Tx_\perp=0.
$$

Then $Hx=x_\perp-x_\parallel$. Subtracting twice the normal component changes its sign while retaining everything parallel to the mirror. A nonzero normal $v$ gives the equivalent formula $H=I-2vv^T/(v^Tv)$, so normalization can be deferred.

For example, take $u=(2,1)^T/\sqrt5$. Its mirror is the [straight line](straight-line.md) $2x_1+x_2=0$, and

$$
H=\begin{pmatrix}-3/5&-4/5\\-4/5&3/5\end{pmatrix},
\qquad
H\begin{pmatrix}3\\4\end{pmatrix}=\begin{pmatrix}-5\\0\end{pmatrix}.
$$

The midpoint of these two [vectors](vector.md) is $(-1,2)^T$, which lies on the mirror; their connecting segment is parallel to its normal. Both [vectors](vector.md) have [Euclidean norm](euclidean-norm.md) five.

<a id="image-a-householder-reflection-reverses-the-normal-component-and-preserves-the-mirror-component"></a>
![](householder-reflection-geometry.png)

**[Figure 15](#image-a-householder-reflection-reverses-the-normal-component-and-preserves-the-mirror-component). A Householder reflection reverses the normal component and preserves the mirror component**. The mirror is $2x_1+x_2=0$. The [vector](vector.md) $(3,4)^T$ becomes $(-5,0)^T$; their midpoint $(-1,2)^T$ is the [orthogonal projection](orthogonal-projection.md) onto the mirror.

Several useful properties follow from this decomposition. The [Householder reflection](householder-transformation.md) is a [symmetric matrix](symmetric-matrix.md) and an [orthogonal matrix](orthogonal-matrix.md):

$$
H^T=H,\qquad H^2=I,\qquad H^TH=I.
$$

Reflecting twice restores the original [vector](vector.md); [Euclidean norms](euclidean-norm.md) and [inner products](inner-product.md) are preserved. The [eigenvalue](eigenvalue.md) is $-1$ along $u$ and $+1$ on $u^\perp$, so $\det H=-1$. A reflection reverses [orientation](orientation-of-a-simplex.md) even though it preserves lengths.

The computational payoff is that the mirror can be chosen to send a whole [vector](vector.md) onto one coordinate axis, eliminating several entries at once. [Householder QR decomposition](householder-qr-decomposition.md) repeats this operation on the remaining parts of successive columns. For a real [symmetric matrix](symmetric-matrix.md), applying the same [Householder reflection](householder-transformation.md) on both sides gives a [matrix similarity](matrix-similarity.md) $HAH$ that preserves symmetry and [eigenvalues](eigenvalue.md); this is the basis of [Householder tridiagonalization](householder-tridiagonalization.md).

Alston S. Householder's 1958 paper _Unitary Triangularization of a Nonsymmetric Matrix_ develops this elimination method. Its motivation includes reducing the arithmetic needed for triangularization while retaining the conditioning advantages of [orthogonal transformations](orthogonal-transformation.md). [Householder (1958), Journal of the ACM 5(4), pp. 339–342: original paper](https://web.stanford.edu/class/cme324/classics/householder.pdf) Over the [complex numbers](complex-number.md), $I-2uu^*$ for a unit $u$ is [Hermitian](hermitian-operator.md) and [unitary](unitary-connection.md), with the star denoting the [conjugate transpose](conjugate-transpose.md); the coordinate-axis construction below is stated for real [vectors](vector.md).

**Table of contents**

- [Householder reflection sending a vector to a coordinate axis](householder-reflection-sending-a-vector-to-a-coordinate-axis.md)
- [Householder QR example in two dimensions](householder-qr-example-in-two-dimensions.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Householder transformation](householder-transformation.md)
- [Orthogonal coordinate reduction of a subspace](orthogonal-coordinate-reduction-of-a-subspace.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/6f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-1/18c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-1/18d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/40e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/40e/b/solution.md)
