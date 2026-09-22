<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

Relative to an origin, the [inertia tensor](../../../../../inertia-tensor.md) is $I_{ij}=\int(r^2\delta_{ij}-r_ir_j)\,dm$, with $\mathbf J=\mathsf I\boldsymbol\omega$. Its orthogonal [eigenvectors](../../../../../eigenvector.md) are [principal axes](../../../../../principal-axis.md), with [eigenvalues](../../../../../eigenvalue.md) the principal moments of inertia. Different components of $\boldsymbol\omega$ are multiplied by different [eigenvalues](../../../../../eigenvalue.md), so [angular momentum](../../../../../angular-momentum.md) need not point along [angular velocity](../../../../../angular-velocity.md).

For a uniform thin disc, radial integration gives $I_z=\int r^2dm=ma^2/2$. The [perpendicular axis theorem](../../../../../perpendicular-axis-theorem.md) and [symmetry](../../../../../symmetry-physics.md) then give $I_x=I_y=I_z/2$, hence

$$
\boxed{I_d=ma^2/4\quad\text{about a diameter}.}
$$

For the [elastic eccentric impact of a thin disc](../../../../../elastic-eccentric-impact-of-a-thin-disc.md), neglect gravity's [impulse](../../../../../impulse.md) and take the pole's [impulse](../../../../../impulse.md) as vertical. Let $z$ point up and let the contact position relative to the centre be $r\hat x$. An upward [impulse](../../../../../impulse.md) $P$ gives

$$
v_C=-u+P/m,\qquad \boldsymbol\omega=-\frac{rP}{I_d}\hat y.
$$

For an elastic impact with a fixed pole, the contact point reverses its normal velocity, so $-u+P/m+r^2P/I_d=+u$. Therefore

$$
\boxed{P=\frac{2mu}{1+4r^2/a^2},\quad
v_C=u\frac{a^2-4r^2}{a^2+4r^2},\quad
\boldsymbol\omega=-\frac{8ur}{a^2+4r^2}\hat y.}
$$

Here $v_C>0$ denotes upward motion; the centre can still move down if $r>a/2$. Substitution gives

$$
\boxed{v_{\rm contact}=v_C+(\boldsymbol\omega\times r\hat x)_z=u.}
$$

This also follows by combining conserved [angular momentum](../../../../../angular-momentum.md) about the fixed contact with conserved [kinetic energy](../../../../../kinetic-energy.md) and selecting the separating, nonzero-impulse solution. At $r=0$ the disc simply rebounds without rotation; at $r=a/2$ its centre is instantaneously stationary. The rebound result concerns the contacting material point immediately after this ideal impact, not its subsequent contact history.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
