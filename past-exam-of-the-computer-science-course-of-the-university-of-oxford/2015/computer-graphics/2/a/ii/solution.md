<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret the given focal point as the centre of [perspective projection](../../../../../../perspective-projection.md), $C=(0,6,-8)$. First translate it to the origin with $H(0,-6,8)$. The direction from $C$ to the world origin is then $(0,-6,8)$, of length 10. Choose the [rotation matrix](../../../../../../rotation-matrix.md) $G(\theta)$ so that this direction becomes $(0,0,10)$:

$$
\cos\theta=\frac45,\qquad \sin\theta=-\frac35,\qquad \theta=-\arctan\frac34.
$$

Indeed, the transformed $y$ component is $-6(4/5)-8(-3/5)=0$, and the transformed $z$ component is $(-6)(-3/5)+8(4/5)=10$. Thus the required mapping, followed by the [perspective divide](../../../../../../perspective-divide.md), is

$$
\boxed{M=K(5)\,G\!\left(-\arctan\frac34\right)\,H(0,-6,8).}
$$

For a world [point](../../../../../../point-geometry.md) $(x,y,z)$, its camera coordinates and projected device coordinates are

$$
X=x,\qquad Y=\frac45y+\frac35z,\qquad Z=10-\frac35y+\frac45z,
$$



$$
(u,v)=\left(\frac{5x}{10-3y/5+4z/5},\frac{4y+3z}{10-3y/5+4z/5}\right),\qquad Z>0.
$$

The world origin projects to $(0,0)$ and lies at camera depth 10. A [point](../../../../../../point-geometry.md) five units along the unit viewing direction from $C$ has camera coordinates $(0,0,5)$, so it lies on the central image plane as expected. Here device coordinates are image-plane coordinates centred on the optical axis; an actual [pixel](../../../../../../pixel.md) viewport would require its own specified scale and offset.

Only [rotations](../../../../../../rotation-mathematics.md) about the $x$-axis are available. Consequently the camera's horizontal axis stays parallel to the world $x$-axis; the viewing direction lies in the world $yz$ plane. The available orientation has pitch but no independent yaw or roll. [Translations](../../../../../../translation-geometry.md) move the camera and the projected origin but cannot supply the missing orientation degrees of freedom.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
