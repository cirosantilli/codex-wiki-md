<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [bacteria](../../../../bacteria.md) disperse by [diffusion](../../../../diffusion.md) with coefficient $D_B$. Their additional [chemotaxis](../../../../chemotaxis.md) [flux](../../../../flux.md) is

$$
J_{B,\mathrm{chem}}=\frac{\chi_B B}{(N_0+N)^2}N_X.
$$

It points up the [nutrient](../../../../nutrient.md) [concentration](../../../../concentration.md) [gradient](../../../../gradient.md), and its negative spatial [derivative](../../../../derivative.md) enters the balance equation. The positive $N_0$ prevents singular sensitivity at zero [nutrient](../../../../nutrient.md) [concentration](../../../../concentration.md); increasing the background [nutrient](../../../../nutrient.md) [concentration](../../../../concentration.md) reduces the drift response to a fixed [gradient](../../../../gradient.md). The [logistic growth equation](../../../../logistic-growth-equation.md) term $rB(1-B/K)$ represents net reproduction with low-population growth rate $r$ and [carrying capacity](../../../../carrying-capacity.md) $K$.

The [nutrient](../../../../nutrient.md) undergoes [diffusion](../../../../diffusion.md) with coefficient $D_N$. Its production term $aB^2/(B_0^2+B^2)$ is an increasing, bounded response to the [bacteria](../../../../bacteria.md), reaching half its maximum $a$ at $B=B_0$. It has the algebraic form of a [Hill equation](../../../../hill-equation.md) with exponent two; the equation alone does not specify a molecular mechanism. The term $dBN$ removes [nutrient](../../../../nutrient.md) at a rate proportional to both [bacteria](../../../../bacteria.md) abundance and [nutrient](../../../../nutrient.md) [concentration](../../../../concentration.md).

The full [fluxes](../../../../flux.md) are

$$
\boxed{J_B=-D_B B_X+\frac{\chi_BB}{(N_0+N)^2}N_X,\qquad J_N=-D_NN_X.}
$$

The homogeneous [Neumann boundary conditions](../../../../neumann-boundary-condition.md) make both [fluxes](../../../../flux.md) vanish at the endpoints, so neither [bacteria](../../../../bacteria.md) nor [nutrient](../../../../nutrient.md) crosses the boundaries. The [initial conditions](../../../../initial-condition.md) specify their starting spatial distributions. This model includes [nutrient](../../../../nutrient.md) production by [bacteria](../../../../bacteria.md), rather than a separate external supply term.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further mathematical biology course of the University of Oxford](../../../split.md)
5. [Further mathematical biology course of the University of Oxford](../../../../further-mathematical-biology-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
