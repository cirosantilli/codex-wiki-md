<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Propagate from one [beam waist](../../../../beam-waist.md) to the other, using the [optical lens](../../../../lens-optics.md) [ray transfer matrix](../../../../ray-transfer-matrix-analysis.md):

$$
M=P(v)L(f)P(u)
=\begin{pmatrix}1-v/f&u+v-uv/f\\-1/f&1-u/f\end{pmatrix}.
$$

[Optical mode matching](../../../../optical-mode-matching.md) requires $q_A=iz_A$ to transform to $q_B=iz_B$. Multiplying the denominator across gives

$$
iz_B(1-u/f-iz_A/f)=(1-v/f)iz_A+u+v-uv/f.
$$

Equating real and imaginary parts and multiplying by $f$ yields

$$
\boxed{v(u-f)+z_Az_B=uf,\qquad
vz_A-z_B(u-f)=z_Af.}
$$

Set $\delta=u-f$. The second equation gives $v=f+(z_B/z_A)\delta$. Substituting this into the first cancels the terms $f\delta$:

$$
\frac{z_B}{z_A}\delta^2+z_Az_B=f^2.
$$

Consequently the two algebraic branches are

$$
\boxed{\delta=\pm\sqrt{\frac{z_A}{z_B}f^2-z_A^2},\qquad
u=f\pm z_A\sqrt{\frac{f^2}{z_Az_B}-1},\qquad
v=f\pm z_B\sqrt{\frac{f^2}{z_Az_B}-1}.}
$$

Equivalently, $u=f+\delta$. The signs in $u$ and $v$ are the same. Real solutions require $\boxed{f^2\geq z_Az_B}$; a converging [optical lens](../../../../lens-optics.md) therefore needs $f\geq\sqrt{z_Az_B}$. At equality $u=v=f$. For the stated arrangement, additionally require $u,v\geq0$ and that the chosen [optical lens](../../../../lens-optics.md) position is accessible outside both [optical resonators](../../../../optical-cavity.md). A negative $v$ is an algebraic virtual-waist solution, not a downstream [beam waist](../../../../beam-waist.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
