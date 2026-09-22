<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [shallow-water approximation](../../../../../../shallow-water-approximation.md) requires $h/L\ll1$, a nearly [hydrostatic pressure](../../../../../../hydrostatic-pressure.md), negligible vertical acceleration, and approximately depth-independent horizontal velocity, concentration, and density. The large [Reynolds number](../../../../../../reynolds-number.md) allows viscous stress to be neglected away from thin boundary layers, while the deep ambient is taken to remain stationary.

For unit channel width, [volume conservation](../../../../../../volume-conservation.md), chemical conservation, and [mass conservation](../../../../../../mass-conservation.md) are respectively

$$
h_t+(uh)_x=w_e-w_d,
$$



$$
(\phi h)_t+(\phi uh)_x=-\phi w_d,
$$

and

$$
(\rho h)_t+(\rho uh)_x=\rho_0w_e-\rho w_d.
$$

Entrained ambient fluid contains no chemical and enters with density $\rho_0$; detrained fluid carries the local concentration and density. The ambient has no horizontal momentum, whereas detrained fluid carries horizontal momentum $\rho u$ per unit volume. The depth-integrated [momentum conservation](../../../../../../momentum-conservation.md) law is therefore

$$
\frac{\partial(\rho uh)}{\partial t}
+\frac{\partial}{\partial x}\left(\rho u^2h+\frac12(\rho-\rho_0)gh^2\right)
=\boxed{-\rho u w_d},
$$

so $M=-\rho u w_d$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
