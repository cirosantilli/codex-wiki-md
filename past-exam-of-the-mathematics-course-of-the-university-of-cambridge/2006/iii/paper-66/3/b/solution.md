<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the equal-time points to estimate [velocity](../../../../../../velocity.md) and [acceleration](../../../../../../acceleration.md) with centered [finite differences](../../../../../../finite-difference-split.md):

$$
V_k\simeq{P_{k+1}-P_{k-1}\over2\Delta t},\qquad a_k\simeq{P_{k+1}-2P_k+P_{k-1}\over(\Delta t)^2}.
$$

At the endpoints use one-sided formulas of the desired order. A differentiated path and its time parametrization can instead supply these quantities. Let $g_k$ denote the gravitational [acceleration](../../../../../../acceleration.md), directed downwards. In the accelerating camera, the effective downward vector is $g_k-a_k$, so the locally felt upward vector is $U_k=a_k-g_k$. For a stationary camera this gives $-g_k$, fixing the sign.

The [apparent-gravity camera frame](../../../../../../apparent-gravity-camera-frame.md) is obtained by [orthogonal projection](../../../../../../orthogonal-projection.md) and a [cross product](../../../../../../cross-product.md):

$$
X_k={V_k\over\|V_k\|},\qquad W_k=U_k-(U_k\cdot X_k)X_k,\qquad Z_k={W_k\over\|W_k\|},\qquad \boxed{Y_k=Z_k\times X_k}.
$$

When $W_k\ne0$, $X_k,Z_k$ are perpendicular [unit vectors](../../../../../../unit-vector.md), and $Y_k$ completes a right-handed [orthonormal basis](../../../../../../orthonormal-basis.md): $X_k\times Y_k=Z_k$. Also $U_k=(U_k\cdot X_k)X_k+\|W_k\|Z_k$, so the felt-up vector lies in the $XZ$ plane, with its transverse component pointing towards positive $Z$.

The stated exclusion of $a_k=g_k$ ensures $U_k\ne0$, but it does not ensure $W_k\ne0$. **If felt-up is parallel to travel, the roll angle is undetermined rather than the construction being impossible.** Every transverse [orthonormal basis](../../../../../../orthonormal-basis.md) then has the required plane property. For continuity, project the previous $Z$ into $X_k^\perp$ and normalize it, using $Y_k=Z_k\times X_k$. If this projection is also too small, choose a coordinate [unit vector](../../../../../../unit-vector.md) least aligned with $X_k$ and project that vector instead. Switch to this transported choice near the parallel case to avoid numerical amplification. A stopped vehicle likewise needs a chosen limiting travel [tangent vector](../../../../../../tangent-vector.md), since its zero [velocity](../../../../../../velocity.md) itself has no direction. None of this requires a [Frenet frame](../../../../../../frenet-frame.md), which can fail where [curvature](../../../../../../curvature.md) vanishes.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
