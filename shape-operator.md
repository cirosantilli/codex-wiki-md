# Shape operator

↑ **Parent:** [Second fundamental form](second-fundamental-form-split.md)

The [shape operator](shape-operator.md) measures how the [unit normal](unit-normal.md) turns as we move along a [smooth surface](smooth-surface.md). A [plane](plane.md) has a constant [unit normal](unit-normal.md), whereas the outward [unit normal](unit-normal.md) of a [sphere](sphere.md) turns in every direction in the [tangent plane](tangent-plane.md). Keeping the direction of this change, rather than just its magnitude, lets one recover the [principal curvatures](principal-curvature.md) and their [principal directions](principal-direction.md).

Choose an [orientation of a surface](orientation-of-a-surface.md) $M\subset\mathbb R^3$, with [Gauss map](gauss-map.md) $N:M\to S^2$. The [shape operator](shape-operator.md) at $p$ is the [linear map](linear-map.md)

$$
S_p=-dN_p:T_pM\to T_pM.
$$

Here $dN_p$ is the [differential](differential-of-a-smooth-map.md) of the [Gauss map](gauss-map.md). Its output belongs to $T_{N(p)}S^2$, identified with $T_pM$ because both are the vector [plane](plane.md) perpendicular to $N(p)$. The minus sign is our convention throughout this branch. [Ghomi, Lecture Notes 9, §2.2: Gauss map and shape operator](https://ghomi.math.gatech.edu/Classes/Math497C/LectureNotes9.pdf)

The [shape operator](shape-operator.md) packages the [second fundamental form](second-fundamental-form-split.md) as an operator using the [inner product](inner-product.md) supplied by the [first fundamental form](first-fundamental-form.md):

$$
II(v,w)=I(S_pv,w).
$$

The [symmetry of the second fundamental form](symmetry-of-the-second-fundamental-form.md) makes the [shape operator](shape-operator.md) a [self-adjoint operator](self-adjoint-operator.md) for this [inner product](inner-product.md). Thus an [orthonormal basis](orthonormal-basis.md) of [principal directions](principal-direction.md) diagonalizes it. In a coordinate [basis](basis.md) $X_u,X_v$ of a [parametric surface](parametric-surface.md), write

$$
A=\begin{pmatrix}E&F\\F&G\end{pmatrix},\qquad B=\begin{pmatrix}e&f\\f&g\end{pmatrix},\qquad [S]=A^{-1}B.
$$

The [matrix](matrix.md) $[S]$ need not be a [symmetric matrix](symmetric-matrix.md) in this coordinate [basis](basis.md): its [self-adjointness](self-adjoint-operator.md) means $A[S]=[S]^TA=B$. Using the [eigenvalues](eigenvalue.md) of $B$ alone gives the [principal curvatures](principal-curvature.md) only when $A$ is the [identity matrix](identity-matrix.md). [Ritter, Geometry of Surfaces, §12.1 and Theorem 12.8: self-adjointness and coordinate matrices](https://people.maths.ox.ac.uk/ritter/geometry-of-surfaces/ritter-geom-surf-67.pdf)

For a worked example, parametrize the lateral surface of an outward-oriented [circular cylinder](circular-cylinder.md) of [radius](radius.md) $R>0$ using circumferential [arc length](arc-length.md) $u$ and axial coordinate $v$:

$$
X(u,v)=(R\cos(u/R),R\sin(u/R),v),\qquad N(u,v)=(\cos(u/R),\sin(u/R),0).
$$

The coordinate [tangent vectors](tangent-vector.md) are an [orthonormal basis](orthonormal-basis.md). Since $N_u=X_u/R$ and $N_v=0$, the [shape operator](shape-operator.md) satisfies

$$
S(X_u)=-\frac1R X_u,\qquad S(X_v)=0,\qquad A=\begin{pmatrix}1&0\\0&1\end{pmatrix},\qquad B=\begin{pmatrix}-1/R&0\\0&0\end{pmatrix}.
$$

Changing to angular coordinate $\varphi=u/R$ gives $A=\operatorname{diag}(R^2,1)$ and $B=\operatorname{diag}(-R,0)$; $A^{-1}B$ still has [eigenvalues](eigenvalue.md) $-1/R,0$. This is why the [first fundamental form](first-fundamental-form.md) must participate in the calculation.

For a [sphere](sphere.md) of [radius](radius.md) $R$ centered at the origin, the outward [unit normal](unit-normal.md) is $N(p)=p/R$. Hence $S_pv=-v/R$, so both [principal curvatures](principal-curvature.md) are $-1/R$. For a [plane](plane.md), $dN=0$ and the [shape operator](shape-operator.md) vanishes. Reversing the [unit normal](unit-normal.md) negates the [shape operator](shape-operator.md) and both [principal curvatures](principal-curvature.md); the [Gaussian curvature](gaussian-curvature.md) remains unchanged while the [mean curvature](mean-curvature.md) changes sign, as in [orientation reversal of surface curvature](orientation-reversal-of-surface-curvature.md).

**Table of contents**

- [Shape operator in a normal direction](shape-operator-in-a-normal-direction.md)
  - [Weingarten formula](weingarten-formula.md)
- [Principal curvature](principal-curvature.md)
  - [Principal direction](principal-direction.md)
  - [Umbilical point](umbilical-point.md)
- [Euclidean invariance of the shape operator](euclidean-invariance-of-the-shape-operator.md)

## ↑ Ancestors (6)

1. [Second fundamental form](second-fundamental-form-split.md)
2. [Differential geometry](differential-geometry-split.md)
3. [Geometry and topology](geometry-and-topology-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (36)

- [A conformal Gauss map does not imply a minimal surface](a-conformal-gauss-map-does-not-imply-a-minimal-surface.md)
- [Differential geometry of surfaces](differential-geometry-of-surfaces.md)
- [Euclidean rigidity of maximal asymptotic volume ratio](euclidean-rigidity-of-maximal-asymptotic-volume-ratio.md)
- [Gaussian curvature](gaussian-curvature.md)
- [Mean curvature](mean-curvature.md)
- [Mean curvature of a sphere and cylinder](mean-curvature-of-a-sphere-and-cylinder.md)
- [Orientation reversal of surface curvature](orientation-reversal-of-surface-curvature.md)
- [Parallel surface](parallel-surface.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-12/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-19/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/2h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/24h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/24h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/23h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/24h/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3/24h/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/24i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/14g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/26f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/26i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/26i/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/25g/a/solution.md)
- [Principal curvature](principal-curvature.md)
- [Principal direction](principal-direction.md)
- [Radial Riccati equation for distance spheres](radial-riccati-equation-for-distance-spheres.md)
- [Shape operator](shape-operator.md)
- [Shape operator in a normal direction](shape-operator-in-a-normal-direction.md)
- [Tangential derivative of a normal field](tangential-derivative-of-a-normal-field.md)
- [Theorema Egregium](theorema-egregium.md)
- [Umbilical point](umbilical-point.md)
- [Weingarten formula](weingarten-formula.md)
