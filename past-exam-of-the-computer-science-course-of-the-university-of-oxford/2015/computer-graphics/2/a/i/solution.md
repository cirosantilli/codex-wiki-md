<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Represent a [point](../../../../../../point-geometry.md) by the column of [homogeneous coordinates](../../../../../../homogeneous-coordinate.md) $(X,Y,Z,1)^T$. The actions of the four [matrices](../../../../../../matrix.md) are:

| Matrix | Geometric action and parameters |
| --- | --- |
| $G(\theta)$ | A [proper rotation](../../../../../../proper-rotation.md) about the $x$-axis: $(X,Y,Z)\mapsto(X,Y\cos\theta-Z\sin\theta,Y\sin\theta+Z\cos\theta)$. The angle $\theta$ is in [radians](../../../../../../radian.md), with the usual right-hand sense. |
| $H(x,y,z)$ | A [translation](../../../../../../translation-geometry.md) by $(x,y,z)$: $(X,Y,Z)\mapsto(X+x,Y+y,Z+z)$. |
| $J(\lambda)$ | Uniform scaling by $\lambda$: $(X,Y,Z)\mapsto(\lambda X,\lambda Y,\lambda Z)$. Positive $\lambda$ gives a [uniform dilation](../../../../../../uniform-dilation.md); $\lambda=0$ collapses the object to the origin; negative $\lambda$ additionally reverses its direction through the origin. |
| $K(f)$ | [Perspective projection](../../../../../../perspective-projection.md) from the origin onto the plane $Z=f$, where $f\ne0$ is the [focal length](../../../../../../focal-length.md) in the chosen coordinate units. |

The last operation produces $(X,Y,Z,Z/f)^T$. It requires a [perspective divide](../../../../../../perspective-divide.md): divide the first three components by the last. For $Z\ne0$,

$$
\boxed{K(f):\quad (X,Y,Z)\longmapsto\left(\frac{fX}{Z},\frac{fY}{Z},f\right).}
$$

This is why the last component of [homogeneous coordinates](../../../../../../homogeneous-coordinate.md) cannot simply be discarded. [Points](../../../../../../point-geometry.md) with $Z=0$ have no finite projected position, and a visible scene normally uses $Z>0$ under this forward-axis convention. The first three transformations leave the last component equal to one and need no nontrivial divide. The displayed $K$ retains no depth variation after division; it describes projection onto the image plane, rather than a complete depth-buffer mapping.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Computer graphics](../../../../computer-graphics-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
