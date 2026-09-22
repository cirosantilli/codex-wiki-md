<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Close the cone with the horizontal disk $D$ at height $h$, and let $V$ be the enclosed solid. The [divergence](../../../../../divergence.md) is

$$
\nabla\cdot\mathbf G=3x^2+2y+3y^2+1=3r^2+2y+1.
$$

The term $2y$ integrates to zero by reflection symmetry of each circular cross-section. Using the [divergence theorem](../../../../../divergence-theorem.md) and [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md), the closed-surface [flux](../../../../../flux.md) is

$$
\int_V\nabla\cdot\mathbf G\,dV
=\int_0^h\int_0^{2\pi}\int_0^{\sqrt2z}(3r^2+1)r\,dr\,d\varphi\,dz
=\int_0^h(6\pi z^4+2\pi z^2)\,dz
=\frac{6\pi h^5}{5}+\frac{2\pi h^3}{3}.
$$

The outward normal on $D$ is $+\widehat{\mathbf z}$, so its [flux](../../../../../flux.md) is its area times $G_z=h$:

$$
\int_D\mathbf G\cdot\mathbf n\,dS=h\,\pi(\sqrt2h)^2=2\pi h^3.
$$

Subtracting this cap contribution gives the required lateral [flux](../../../../../flux.md):

$$
\boxed{\int_A\mathbf G\cdot d\mathbf A=\frac{6\pi h^5}{5}-\frac{4\pi h^3}{3}.}
$$

This is [conical flux by closing with a cap](../../../../../conical-flux-by-closing-with-a-cap.md). The normal convention matters: on the lateral cone the outward normal points radially outwards and partly downwards, so the $G_z$ contribution to the lateral [flux](../../../../../flux.md) is negative. To justify applying the theorem at the vertex, truncate a small tip and take its size to zero; the extra [flux](../../../../../flux.md) vanishes because $\mathbf G$ is regular there.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
