<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Define the [transformed Eulerian mean](../../../../../../transformed-eulerian-mean.md) circulation by

$$
\boxed{
\overline v_a^*=\overline v_a-\frac1{N^2}
\frac{\partial\overline{v'\sigma'}}{\partial z},
\qquad
\overline w_a^*=\overline w_a+\frac1{N^2}
\frac{\partial\overline{v'\sigma'}}{\partial y}.}
$$

The added terms form a nondivergent eddy-induced circulation, so $\partial_y\overline v_a^*+\partial_z\overline w_a^*=0$. The buoyancy equation becomes

$$
\overline\sigma_t+N^2\overline w_a^*=0.
$$

Substituting $\overline v_a=\overline v_a^*+N^{-2}\partial_z\overline{v'\sigma'}$ into the momentum equation gives

$$
\overline u_t-\beta y\overline v_a^*
=\frac{\partial F^{(y)}}{\partial y}
+\frac{\partial F^{(z)}}{\partial z},
$$

where the components of the [Eliassen–Palm flux](../../../../../../eliassen-palm-flux.md) are

$$
\boxed{
F^{(y)}=-\overline{u'v'},
\qquad
F^{(z)}=-\overline{u'w'}
+\frac{\beta y}{N^2}\overline{v'\sigma'}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
