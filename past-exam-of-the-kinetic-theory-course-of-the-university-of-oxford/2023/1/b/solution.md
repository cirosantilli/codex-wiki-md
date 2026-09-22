<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathbf A_i=\sum_{j\ne i}K_{ij}(\mathbf v_j-\mathbf v_i)$. Conservation of [probability](../../../../probability.md) in the full [phase space](../../../../phase-space.md) gives the [dissipative Liouville equation](../../../../dissipative-liouville-equation.md)

$$
\boxed{\partial_t\varrho+\sum_{i=1}^N\nabla_{\mathbf x_i}\cdot(\mathbf v_i\varrho)+\sum_{i=1}^N\nabla_{\mathbf v_i}\cdot(\mathbf A_i\varrho)=0.}
$$

Normalize $\int\varrho\,\prod_i d^3x_i\,d^3v_i=1$. Decay at infinity makes all boundary fluxes vanish, so the equation preserves this [normalization of a probability distribution](../../../../normalization-of-a-probability-distribution.md).

Unlike the [Hamiltonian Liouville equation](../../../../hamiltonian-liouville-equation.md), this transport has nonzero [phase-space divergence](../../../../phase-space-divergence.md). In three [dimensions](../../../../dimension-vector-space.md),

$$
\nabla_{\mathbf v_i}\cdot\mathbf A_i=-3\sum_{j\ne i}K_{ij},\qquad
\partial_t\varrho+\sum_i\left(\mathbf v_i\cdot\nabla_{\mathbf x_i}\varrho+\mathbf A_i\cdot\nabla_{\mathbf v_i}\varrho\right)=3\varrho\sum_i\sum_{j\ne i}K_{ij}.
$$

The [probability density](../../../../probability-density.md) increases along a contracting [characteristic flow map](../../../../characteristic-flow-map.md); setting its material derivative to zero would lose conservation of [probability](../../../../probability.md). The $j=i$ force is identically zero, including its derivative, which is why the last sums exclude it.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
