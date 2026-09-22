<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The required [Hamilton-Jacobi equation](../../../../hamilton-jacobi-equation.md) is

$$
\boxed{S_t+\frac1{2m}(S_x^2+S_y^2+S_z^2)+mgz=0.}
$$

Because $x,y$ and time are cyclic in the [Hamiltonian](../../../../hamiltonian.md), use separation $S=ax+by-Et+W(z)$. The remaining equation is

$$
(W')^2=2m(E-mgz)-a^2-b^2\equiv Q(z).
$$

For $g\ne0$, each sign branch has the separated complete integral

$$
\boxed{S=ax+by-Et-\frac{s}{3m^2g}[2m(E-mgz)-a^2-b^2]^{3/2},\qquad s=\pm1.}
$$

It is real in the classically allowed region $Q\ge0$, and $p_z=s\sqrt Q$. At a turning point one matches the ascending and descending branches. If $g=0$, the integral is simply $W=p_zz$ with constant $p_z$.

A convenient equivalent complete integral, expressed using initial-momentum constants $\boldsymbol\alpha$, is globally polynomial in time:

$$
\boxed{\begin{aligned}
S={}&\alpha_xx+\alpha_yy+(\alpha_z-mgt)z
-\frac{\alpha_x^2+\alpha_y^2+\alpha_z^2}{2m}t\\
&+\frac{\alpha_zg}{2}t^2-\frac{mg^2}{6}t^3.
\end{aligned}}
$$

Substitution verifies that its time derivative cancels the kinetic term and $mgz$. It avoids a square-root branch change when extracting the complete [trajectory](../../../../trajectory.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the classical mechanics course of Part B of the physics course of the University of Oxford](../../../split.md)
5. [Classical mechanics course of Part B of the physics course of the University of Oxford](../../../../classical-mechanics-course-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../c/solution.md)
