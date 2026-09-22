<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define mean streaming [velocity](../../../../velocity.md) $u_i=\overline{v_i}$ and the [velocity dispersion](../../../../velocity-dispersion.md) tensor $\sigma_{ij}^2=\overline{(v_i-u_i)(v_j-u_j)}=\overline{v_iv_j}-u_iu_j$. The zeroth [velocity](../../../../velocity.md) moment of the steady [Collisionless Boltzmann equation](../../../../collisionless-boltzmann-equation.md) gives the [continuity equation](../../../../continuity-equation.md) $\sum_i\partial_i(nu_i)=0$. Therefore

$$
\sum_i\partial_i(nu_iu_j)=n\sum_i u_i\partial_i u_j.
$$

Substituting in [a](../a.md) yields the standard steady [Jeans equations](../../../../jeans-equation.md):

$$
\boxed{\sum_i u_i\frac{\partial u_j}{\partial x_i}=-\frac{\partial\Phi}{\partial x_j}-\frac1n\sum_i\frac{\partial(n\sigma_{ij}^2)}{\partial x_i},\qquad j=1,2,3.}
$$

The unsteady version adds $\partial_tu_j$ on the left. Defining the stellar [pressure tensor](../../../../pressure-tensor.md) $P_{ij}=\rho\sigma_{ij}^2$ makes the analogy with fluid momentum balance explicit. The off-diagonal terms are correlations between random [velocity](../../../../velocity.md) components; they need not vanish or equal the diagonal terms.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
