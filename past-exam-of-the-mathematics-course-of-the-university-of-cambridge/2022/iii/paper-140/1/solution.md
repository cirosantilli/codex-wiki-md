<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use polar coordinates $z_j=r_je^{i\theta_j}$ on each complex coordinate plane. On $S^3$, where $r_1^2+r_2^2=1$,

$$
\alpha_s=\frac12(r_1^2d\theta_1+sr_2^2d\theta_2),
\qquad
d\alpha_s=r_1dr_1\wedge d\theta_1+sr_2dr_2\wedge d\theta_2.
$$

Direct substitution shows that $\alpha_s\wedge d\alpha_s$ is nowhere zero for $s>0$, so $\alpha_s$ is a [contact form](../../../../../contact-form.md).

The vector field

$$
R_s=2\frac{\partial}{\partial\theta_1}+\frac2s\frac{\partial}{\partial\theta_2}
$$

satisfies $\alpha_s(R_s)=r_1^2+r_2^2=1$ and $\iota_{R_s}d\alpha_s=0$ on tangent vectors to the sphere. It is therefore the [Reeb vector field](../../../../../reeb-vector-field.md). Its flow is

$$
(z_1,z_2)\longmapsto(e^{2it}z_1,e^{2it/s}z_2).
$$

If both coordinates are nonzero, an orbit closes only if the two angular frequencies have rational ratio, equivalently if $s\in\mathbb Q$. For irrational $s$, the only closed orbits are $\{z_2=0\}$ and $\{z_1=0\}$, the two coordinate circles. This is the [irrational contact ellipsoid flow on the three-sphere](../../../../../irrational-contact-ellipsoid-flow-on-the-three-sphere.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 140](../../paper-140-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
