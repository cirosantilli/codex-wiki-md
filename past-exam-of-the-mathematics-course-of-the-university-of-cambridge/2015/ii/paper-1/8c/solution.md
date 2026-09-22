<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

Relative positions and velocities measured from galaxy $A$ are $r_B-r_A$ and $v_B-v_A$. [Spatial homogeneity](../../../../../spatial-homogeneity.md) says that the same position-to-relative-velocity rule applies from every galaxy. Thus $v(r_B-r_A)=v(r_B-r_O)-v(r_A-r_O)$. Taking $r_O=0$ and putting $r_B=x+y$, $r_A=y$ gives additivity $v(x+y)=v(x)+v(y)$. For a continuous physical velocity field, additivity implies rational homogeneity and, by continuity, real homogeneity. Therefore

$$
\boxed{v(r)=Hr}
$$

for a position-independent [matrix](../../../../../matrix.md) $H$. Regularity is necessary to exclude pathological discontinuous additive functions.

Decompose the given [matrix](../../../../../matrix.md) as $H=(5D/t)I+(D/t)W$, where

$$
W=\begin{pmatrix}0&-1&-2\\1&0&-1\\2&1&0\end{pmatrix}.
$$

Its symmetric part is isotropic: no [cosmological shear](../../../../../cosmological-shear.md), expansion scalar $\nabla\cdot v=15D/t$, and linear scale factor proportional to $t^{5D}$ for $t>0$. Its antisymmetric part is rigid rotation with [angular velocity](../../../../../angular-velocity.md)

$$
\boxed{\boldsymbol\omega(t)=\frac D t(1,-2,1),\qquad|\boldsymbol\omega|=\frac{\sqrt6D}{t}}.
$$

The [vorticity](../../../../../vorticity.md) is $2\boldsymbol\omega$. Comoving separations obey

$$
r(t)=\left(\frac t{t_0}\right)^{5D}
\exp\!\left[D\log(t/t_0)W\right]r(t_0).
$$

Thus all distances grow by the same power, volumes grow as $t^{15D}$, and the pattern rotates about the fixed axis $(1,-2,1)$ through angle $\sqrt6D\log(t/t_0)$. Homogeneity alone permits this rotation; full cosmological isotropy would not.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
