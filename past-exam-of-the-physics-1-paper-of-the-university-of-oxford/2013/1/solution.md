<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [parallel axis theorem](../../../parallel-axis-theorem.md) states $I=I_G+Md^2$ for parallel axes separated by $d$, with the reference axis through the [centre of mass](../../../center-of-mass.md). The [perpendicular axis theorem](../../../perpendicular-axis-theorem.md) states $I_z=I_x+I_y$ for a planar lamina in the $xy$ plane, about mutually perpendicular axes through one point. It does not apply directly to a three-dimensional solid.

For the [transverse moment of inertia of a uniform solid cylinder](../../../transverse-moment-of-inertia-of-a-uniform-solid-cylinder.md), divide the cylinder into thin disks at axial positions $z\in[-h/2,h/2]$. Symmetry and the [perpendicular axis theorem](../../../perpendicular-axis-theorem.md) give the diametral [moment of inertia](../../../moment-of-inertia.md) $r^2\,dM/4$ of each disk; the [parallel axis theorem](../../../parallel-axis-theorem.md) adds $z^2\,dM$. Hence

$$
I_\perp=\frac Mh\int_{-h/2}^{h/2}\left(\frac{r^2}{4}+z^2\right)dz,\qquad
\boxed{I_\perp=\frac M{12}(3r^2+h^2).}
$$

The thin-disk limit is $Mr^2/4$, while the slender-rod limit is $Mh^2/12$.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2013](../../2013-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
