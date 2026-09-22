<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Setting $I=0$ in [cylindrical magnetostatic pressure balance](../../../../../../cylindrical-magnetostatic-pressure-balance.md) gives $p+B_z^2/(8\pi)=\mathrm{constant}$. The axial boundary value sets this constant to $p_0$. Thus the [magnetic pressure support with vanishing axial field](../../../../../../magnetic-pressure-support-with-vanishing-axial-field.md) solution is

$$
\boxed{B_z(R)=\sigma\sqrt{8\pi p_0}\sqrt{1-e^{-R^2/a^2}},\qquad \sigma=\pm1.}
$$

The azimuthal component of the magnetostatic [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md) gives

$$
\boxed{j_\phi(R)=-\sigma\frac{c\sqrt{8\pi p_0}}{4\pi a^2}
\frac{R e^{-R^2/a^2}}{\sqrt{1-e^{-R^2/a^2}}}.}
$$

Since $1-e^{-R^2/a^2}=R^2/a^2+O(R^4)$, the radial limit is

$$
\boxed{\lim_{R\downarrow0}j_\phi(R)=-\sigma\frac{c\sqrt{8\pi p_0}}{4\pi a}.}
$$

There is a regularity subtlety: $B_z\sim\sigma\sqrt{8\pi p_0}R/a$ is not a [smooth function](../../../../../../smooth-function.md) of Cartesian position at the axis, and the nonzero limiting $j_\phi$ multiplies an azimuthal unit vector with no unique direction there. These formulas solve the radial problem for $R>0$ and give the requested scalar limit, but the data in this part do not admit the fully smooth vector-field regularity assumed in part (a).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
