<h1 id="17c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $R=|\mathbf p|>a$. In SI units, the exterior [electrostatic potential](../../../../../../electric-potential.md) solves

$$
\Delta\Phi=-\frac q{\varepsilon_0}\delta(\mathbf x-\mathbf p)\quad(|\mathbf x|>a),\qquad
\Phi=0\quad(|\mathbf x|=a),\qquad \Phi\to0\quad(|\mathbf x|\to\infty),
$$

with the point-charge singularity $q/(4\pi\varepsilon_0|\mathbf x-\mathbf p|)$. The [image charge for a grounded conducting sphere](../../../../../../image-charge-for-a-grounded-conducting-sphere.md) choices

$$
\boxed{\mathbf p'=\frac{a^2}{R^2}\mathbf p,\qquad q'=-\frac aR q}
$$

lie inside the sphere. On $|\mathbf x|=a$, direct squaring gives $|\mathbf x-\mathbf p'|=(a/R)|\mathbf x-\mathbf p|$. Therefore

$$
\Phi(\mathbf x)=\frac1{4\pi\varepsilon_0}\left(\frac q{|\mathbf x-\mathbf p|}+\frac{q'}{|\mathbf x-\mathbf p'|}\right)
$$

satisfies the source equation, grounded boundary value and decay at infinity. The [Uniqueness of the Dirichlet problem](../../../../../../uniqueness-of-the-dirichlet-problem.md), applied to the harmonic difference with its singularity removed, identifies this with the physical exterior potential. Thus its gradient gives the required exterior [electric field](../../../../../../electric-field.md).

The charge feels the induced field, equivalently the field of the [image charge](../../../../../../image-charge.md), excluding its own singular field. Their separation is $(R^2-a^2)/R$, so [Coulomb's law](../../../../../../coulomb-s-law.md) gives

$$
\boxed{\mathbf F=-\frac{q^2aR}{4\pi\varepsilon_0(R^2-a^2)^2}\,\frac{\mathbf p}{R}.}
$$

Its magnitude is $q^2aR/[4\pi\varepsilon_0(R^2-a^2)^2]$ and its direction is toward the sphere's center, independent of the sign of $q$. No factor one-half belongs in this force; that factor occurs in induced electrostatic energy instead.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [17C](../../17c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
