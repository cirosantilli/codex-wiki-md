<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the paper's [Fubini-Study form](../../../../../../fubini-study-form.md) normalization $\widetilde\omega_{FS}=\frac{i}{2}\partial\overline\partial\log(1+|z|^2)$, the [Hamiltonian vector field](../../../../../../hamiltonian-vector-field.md) convention $\iota_{X_H}\omega=dH$, and the [Lie algebra](../../../../../../lie-algebra-split.md) generator whose [circle](../../../../../../circle.md) action is $e^{i\theta}$. Write $D=|z_0|^2+|z_1|^2+|z_2|^2$. The normalized [moment map](../../../../../../moment-map.md) for the [torus](../../../../../../torus.md) action is

$$
\boxed{\phi([z_0,z_1,z_2])=-\frac1{2D}\bigl(|z_1|^2,|z_2|^2\bigr).}
$$

The [moment map](../../../../../../moment-map.md) image is the filled triangle

$$
\boxed{\phi(\mathbb{CP}^2)=\{(u,v):u\leq0,\ v\leq0,\ u+v\geq-\tfrac12\}.}
$$

Indeed, the three quantities $|z_j|^2/D$ are nonnegative and add to one, and any such triple is realized by choosing their square roots as [homogeneous coordinates](../../../../../../homogeneous-coordinate.md).

For the diagonal [circle](../../../../../../circle.md) action, a point in the [fixed-point set](../../../../../../fixed-point-set.md) satisfies $[z_0,tz_1,tz_2]=[z_0,z_1,z_2]$ for every $t\in S^1$. If $z_0\ne0$, the projective scaling must be one, forcing $z_1=z_2=0$. If $z_0=0$, all coordinates are scaled together. Therefore

$$
\boxed{\operatorname{Fix}(S^1)=\{[1,0,0]\}\ \sqcup\ \{[0,z_1,z_2]\}\cong\{\mathrm{point}\}\sqcup\mathbb{CP}^1.}
$$

By part (b), the diagonal [moment map](../../../../../../moment-map.md) is

$$
\boxed{\mu([z])=-\frac{|z_1|^2+|z_2|^2}{2D},\qquad\mu(\mathbb{CP}^2)=[-\tfrac12,0].}
$$

The factor $1/2$ follows from the specified [Fubini-Study form](../../../../../../fubini-study-form.md), not the integral normalization in the linked general article. For example, in one affine complex coordinate $w=re^{i\theta}$ the [symplectic form](../../../../../../symplectic-form.md) is $r(1+r^2)^{-2}dr\wedge d\theta$, whose [interior product of a differential form](../../../../../../interior-product.md) with $\partial_\theta$ is $-r(1+r^2)^{-2}dr=d[-r^2/(2(1+r^2))]$. Choosing the generator $e^{2\pi it}$ rescales all [moment maps](../../../../../../moment-map.md) by $2\pi$; reversing the defining sign reverses their signs. The negative level in parts (d) and (e) uses the convention displayed here.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 140](../../../paper-140-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
