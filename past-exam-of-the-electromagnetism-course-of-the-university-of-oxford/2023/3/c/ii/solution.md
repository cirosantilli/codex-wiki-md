<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the sign $s=\pm1$ to label a [point charge](../../../../../point-charge.md) $sq$ at $s\mathbf p/(2q)$, with [velocity](../../../../../velocity.md) $s\mathbf p'/(2q)$. All quantities on the right below are evaluated at $t_0=t-r/c$. To first order,

$$
\mathbf R_s=\mathbf r-\frac{s\mathbf p}{2q}+O(q^{-2}),\qquad
R_s=r-\frac{s\mathbf n\cdot\mathbf p}{2q}+O(q^{-2}),\qquad
\mathbf v_s=\frac{s\mathbf p'}{2q}+O(q^{-2}).
$$

The denominator in each [Liénard–Wiechert potential](../../../../../lienard-wiechert-potential.md) therefore expands as

$$
D_s=R_s-\mathbf R_s\cdot\mathbf v_s/c
=r-\frac{s}{2q}\left(\mathbf n\cdot\mathbf p+\frac{\mathbf r\cdot\mathbf p'}c\right)+O(q^{-2}),
$$

so

$$
\frac1{D_s}=\frac1r+\frac{s}{2qr^2}
\left(\mathbf n\cdot\mathbf p+\frac{\mathbf r\cdot\mathbf p'}c\right)+O(q^{-2}).
$$

In the sum of the two [electric potentials](../../../../../electric-potential.md), the $q/r$ terms cancel and the finite terms add. This gives the [retarded potentials of a point electric dipole](../../../../../retarded-potentials-of-a-point-electric-dipole.md):

$$
\boxed{\phi(\mathbf r,t)=\frac1{4\pi\epsilon_0}
\left(\frac{\mathbf r\cdot\mathbf p(t_0)}{r^3}
+\frac{\mathbf r\cdot\mathbf p'(t_0)}{cr^2}\right),\qquad r>0.}
$$

For the [magnetic vector potential](../../../../../magnetic-vector-potential.md), the signed [electric charge](../../../../../electric-charge-split.md) and signed [velocity](../../../../../velocity.md) multiply to give the same sign for both contributions:

$$
\mathbf A=\frac1{4\pi\epsilon_0c^2}\sum_{s=\pm1}\frac{sq\,\mathbf v_s}{D_s}
\longrightarrow\frac{\mathbf p'}{4\pi\epsilon_0c^2r}.
$$

Since $\mu_0\epsilon_0c^2=1$,

$$
\boxed{\mathbf A(\mathbf r,t)=\frac{\mu_0}{4\pi r}\mathbf p'(t_0).}
$$

The $\mathbf p'$ term in the [electric potential](../../../../../electric-potential.md) arises from the moving-source denominator and remains finite in the point-[electric dipole](../../../../../electric-dipole.md) limit; discarding it would fail to give the full retarded [electric field](../../../../../electric-field-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
