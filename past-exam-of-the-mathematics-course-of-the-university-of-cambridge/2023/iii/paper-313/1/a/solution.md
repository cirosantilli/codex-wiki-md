<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [classical field-theory soliton](../../../../../../classical-field-theory-soliton-split.md) is a smooth, spatially localized, finite-energy solution which retains its identity under time evolution and is stable against small perturbations, commonly because of a [topological charge](../../../../../../topological-charge.md) or a balance between energy terms with different scaling behavior.

For a static field write

$$
E=E_2+E_4+E_0,
$$

where

$$
E_2=\frac12\int|\nabla\phi|^2d^Dx,
\qquad
E_4=\kappa^2\int|\nabla\phi|^4d^Dx,
\qquad
E_0=\int U(\phi)d^Dx.
$$

Under the [Derrick scaling](../../../../../../derrick-scaling.md) $\phi_\lambda(\mathbf x)=\phi(\lambda\mathbf x)$, a [change of variables](../../../../../../change-of-variables-formula.md) gives

$$
E(\lambda)=\lambda^{2-D}E_2
+\lambda^{4-D}E_4+\lambda^{-D}E_0.
$$

A static solution must be stationary under this variation, so the [Derrick virial identity](../../../../../../derrick-virial-identity.md) is

$$
\boxed{(2-D)E_2+(4-D)E_4-DE_0=0}.
$$

All three energies are nonnegative. For $D\geq4$, every coefficient is nonpositive and the coefficient of the strictly positive $E_2$ of any nonconstant field is negative. The identity is impossible. Thus, when the quartic-gradient term is available,

$$
\boxed{D\geq4\quad\Longrightarrow\quad\text{no nontrivial static soliton}.}
$$

For $D=2$ or $3$, the $E_4$ term has the opposite sign to at least one other term and the [Derrick theorem](../../../../../../derrick-s-theorem.md) does not rule out a soliton. If $\kappa=0$ from the outset, the identity reduces to $(2-D)E_2-DE_0=0$, recovering the stronger standard obstruction for $D\geq2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 313](../../../paper-313-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
