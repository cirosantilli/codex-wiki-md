<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For single-shot [ray tracing](../../../../../ray-tracing-computer-graphics.md), construct one primary [ray](../../../../../ray-geometry.md) per [pixel](../../../../../pixel.md), normally through its centre on the image plane, with the camera centre as origin for [perspective projection](../../../../../perspective-projection.md). Transform the [ray](../../../../../ray-geometry.md) into the scene's coordinates, or consistently transform all the scene geometry into camera coordinates.

Intersect that primary [ray](../../../../../ray-geometry.md) with the scene's [triangles](../../../../../triangle.md), using part (c), and retain the accepted hit with the smallest nonnegative parameter $\lambda$. This nearest-hit selection supplies visibility: farther surfaces cannot show through the first opaque surface. If there is no hit, write the background colour. At a hit $p$, obtain its material colour and front [unit normal vector](../../../../../unit-normal.md) and set $\hat V$ toward the camera.

For each point light at $\ell_j$, form $\hat L_j=(\ell_j-p)/\|\ell_j-p\|$, calculate the [specular reflection](../../../../../specular-reflection.md) direction, and evaluate its diffuse and specular contributions using the [Phong reflection model](../../../../../phong-reflection-model.md). Sum the contributions and add ambient illumination once:

$$
\boxed{I(p)=k_aI_a+\sum_j I_j(p)\left[k_d\max(0,\hat N\cdot\hat L_j)+k_s\chi_j\max(0,\hat R_j\cdot\hat V)^n\right].}
$$

The coloured surface can supply colour-dependent diffuse weights, and each source can have its own colour. Convert the result into the output image's colour encoding and range. Single-shot here means direct local shading after one primary visibility [ray](../../../../../ray-geometry.md); no reflected or transmitted secondary viewing rays are followed. Part (e) adds secondary visibility queries for the lights.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Computer graphics](../../../computer-graphics-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
