# Divergence and curl from orthogonal coordinate gradients

↑ **Parent:** [Orthogonal coordinates](orthogonal-coordinates.md)

For a right-handed regular system of [orthogonal coordinates](orthogonal-coordinates.md), the [gradient in orthogonal coordinates](gradient-in-orthogonal-coordinates.md) gives $\nabla u_i=\mathbf e_i/h_i$. Thus $\phi\mathbf e_1=(\phi h_1)\nabla u_1$, and the [curl](curl.md) product rule gives

$$
\nabla\times(\phi\mathbf e_1)=\nabla(\phi h_1)\times\nabla u_1=\frac{\mathbf e_2}{h_1h_3}\partial_{u_3}(\phi h_1)-\frac{\mathbf e_3}{h_1h_2}\partial_{u_2}(\phi h_1).
$$

Also $\nabla u_2\times\nabla u_3=\mathbf e_1/(h_2h_3)$ and the [divergence](divergence.md) of this cross product is zero, by the divergence-of-a-cross-product identity and the vanishing curl of each gradient. Applying the divergence product rule to $\phi\mathbf e_1=(\phi h_2h_3)(\nabla u_2\times\nabla u_3)$ gives

$$
\nabla\cdot(\phi\mathbf e_1)=\frac{\partial_{u_1}(\phi h_2h_3)}{h_1h_2h_3}.
$$

Cyclic permutation and addition give the full component formulas for any [vector field](vector-field.md). This derivation accounts for the varying coordinate basis without differentiating its unit vectors explicitly. The factors $h_i>0$ are [scale factors of orthogonal coordinates](scale-factors-of-orthogonal-coordinates.md); the chart must avoid coordinate singularities.

## ↑ Ancestors (9)

1. [Orthogonal coordinates](orthogonal-coordinates.md)
2. [Change of variables formula](change-of-variables-formula.md)
3. [Multivariable calculus](multivariable-calculus-split.md)
4. [Calculus](calculus-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/1/solution.md)
