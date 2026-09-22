<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

Choose an origin near the bounded loop and write $\mathbf r'$ for the source position. The [magnetic vector potential](../../../../../magnetic-vector-potential.md) and its far-field [multipole expansion](../../../../../electric-multipole-expansion.md) are

$$
\mathbf A(\mathbf r)=\frac{\mu_0 I}{4\pi}\oint_C\frac{d\mathbf r'}{|\mathbf r-\mathbf r'|},\qquad
\frac1{|\mathbf r-\mathbf r'|}=\frac1r+\frac{\mathbf r\cdot\mathbf r'}{r^3}+O(r^{-3}),
$$

with the loop held fixed as $r=|\mathbf r|\to\infty$. The first term integrates to zero since $C$ is closed. Define its oriented [vector area](../../../../../vector-area.md) by

$$
\mathbf S=\frac12\oint_C\mathbf r'\times d\mathbf r'=\int_\Sigma\mathbf n\,dS.
$$

The second equality is [Stokes theorem](../../../../../stokes-theorem.md), applied componentwise to any oriented spanning surface. In particular the [vector area](../../../../../vector-area.md) is independent of the choice of spanning surface. From $\oint_C d(r'_i r'_j)=0$, the matrix $\oint_C r'_i\,dr'_j$ is antisymmetric, which gives $\oint_C(\mathbf r\cdot\mathbf r')d\mathbf r'=\mathbf S\times\mathbf r$. Hence

$$
\boxed{\mathbf m=I\mathbf S,\qquad \mathbf A(\mathbf r)=\frac{\mu_0}{4\pi}\frac{\mathbf m\times\mathbf r}{r^3}+O(r^{-3})}.
$$

The orientation follows the current by the [right-hand rule](../../../../../right-hand-rule.md). For $r\ne0$, taking the [curl](../../../../../curl.md) of this leading [magnetic vector potential](../../../../../magnetic-vector-potential.md) gives the [magnetic dipole field](../../../../../magnetic-dipole-field.md)

$$
\boxed{\mathbf B(\mathbf r)=\frac{\mu_0}{4\pi}\left(\frac{3(\mathbf m\cdot\mathbf r)\mathbf r}{r^5}-\frac{\mathbf m}{r^3}\right)+O(r^{-4})}.
$$

For a planar loop, $\mathbf S$ is the signed area times the unit [normal vector](../../../../../normal-vector.md). For a nonplanar loop it is the oriented [vector area](../../../../../vector-area.md), rather than the scalar area of an arbitrarily chosen surface.

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
