<h1 id="a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every point in the affine search space is uniquely $x_k=x_0+V_ky$, since the columns of $V_k$ form a basis. Its [linear-system residual](../../../../../linear-system-residual.md) is $r_k=r_0-AV_ky$, so minimizing the residual is exactly the [linear least-squares problem](../../../../../linear-least-squares-problem.md) $\min_y\|r_0-AV_ky\|_2$.

Use the standard starting choice $v_1=r_0/\|r_0\|_2$ and an orthonormal extended basis $V_{k+1}$. If $AV_k=V_{k+1}L_k$, then $r_0=V_{k+1}(\|r_0\|_2e_1)$ and orthonormality gives

$$
\boxed{\|r_0-AV_ky\|_2=\big\|\|r_0\|_2e_1-L_ky\big\|_2.}
$$

The starting-vector choice is needed for this particular $e_1$ representation; an arbitrary orthonormal basis need not have those initial coordinates.

The [Arnoldi iteration](../../../../../arnoldi-iteration.md) constructs the basis. At column $j$, orthogonalize $Av_j$ against $v_1,\ldots,v_j$, recording coefficients $h_{ij}=v_i^TAv_j$; normalize the remaining vector with $h_{j+1,j}$ to get $v_{j+1}$. This makes $L_k$ an upper [Hessenberg matrix](../../../../../hessenberg-matrix.md) of size $(k+1)\times k$. The resulting [GMRES](../../../../../generalized-minimal-residual-method.md) algorithm starts from $x_0,r_0$, grows this Arnoldi basis, solves the small least-squares problem, and sets $x_k=x_0+V_ky$. Its small residual norm provides the stopping test. Incremental [Givens rotations](../../../../../givens-rotation.md) efficiently update the small [QR decomposition](../../../../../qr-decomposition.md) instead of solving it anew. Zero initial residual means the system is already solved; Arnoldi breakdown gives an invariant subspace and, for nonsingular $A$, permits exact solution within it.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
