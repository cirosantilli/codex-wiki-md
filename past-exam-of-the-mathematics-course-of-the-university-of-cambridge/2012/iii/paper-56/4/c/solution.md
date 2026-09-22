<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Extract the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) from $\Theta^a{}_b=\tfrac12R^a{}_{bcd}e^c\wedge e^d$ using the [curvature 2-forms](../../../../../../curvature-2-form.md) just computed. Contraction $R_{bd}=R^a{}_{bad}$ gives the diagonal [Ricci tensor](../../../../../../ricci-tensor.md) in the [orthonormal coframe](../../../../../../orthonormal-coframe-in-spacetime.md):

$$
R_{00}=q+2a^2,\qquad R_{11}=R_{22}=-(q+2a^2),\qquad R_{33}=-3q,\qquad R=-6q-6a^2.
$$

For example, the $00$ component receives $a^2$ from each of the $1$ and $2$ directions and $q$ from direction $3$. The signs in the spatial components reflect the same Lorentzian index lowering used for the [connection 1-forms](../../../../../../connection-1-form-split.md).

For a [null vector](../../../../../../null-vector.md) $k$ in this frame, $(k^0)^2=(k^1)^2+(k^2)^2+(k^3)^2$. Therefore

$$
R_{ab}k^ak^b=(q+2a^2)\bigl((k^0)^2-(k^1)^2-(k^2)^2\bigr)-3q(k^3)^2=2(a^2-q)(k^3)^2=-2a'(k^3)^2.
$$

The [Einstein field equations](../../../../../../einstein-field-equations.md) imply $8\pi T_{ab}k^ak^b=R_{ab}k^ak^b$, since the metric term vanishes for a [null vector](../../../../../../null-vector.md); an included cosmological-constant term would also vanish. Choose $k^a=(1,0,0,1)$ and apply the [null energy condition](../../../../../../null-energy-condition.md). It follows that

$$
\boxed{\frac{d^2}{dz^2}\log A=a'=\frac{A''}A-\frac{(A')^2}{A^2}\le0.}
$$

Conversely, this inequality makes the same contraction nonnegative for every [null vector](../../../../../../null-vector.md), so it is exactly the [null energy condition for a planar warped spacetime](../../../../../../null-energy-condition-for-a-planar-warped-spacetime.md) when its matter [stress-energy tensor](../../../../../../stress-energy-tensor.md) is defined by the [Einstein field equations](../../../../../../einstein-field-equations.md). Null vectors tangent to the planar slices saturate the condition. As checks, constant $A$ gives flat spacetime and $A=e^{bz}$ gives constant negative sectional curvature with $a'=0$, also saturating it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
