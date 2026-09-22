<h1 id="k/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The momentum of a [material volume](../../../../material-volume.md) $V(t)$ is $\int_{V(t)}\rho\mathbf u\,dV$. [Newton's second law](../../../../newton-s-second-law.md) equates its time derivative to the [pressure](../../../../pressure-split.md) force and [gravity](../../../../gravity.md):

$$
\frac d{dt}\int_{V(t)}\rho\mathbf u\,dV
=-\int_{\partial V(t)}p\mathbf n\,dS+\int_{V(t)}\rho\mathbf g\,dV.
$$

Apply the given [Reynolds transport theorem](../../../../reynolds-transport-theorem.md) componentwise to the left side, and the [divergence theorem](../../../../divergence-theorem.md) to the [pressure](../../../../pressure-split.md) term. Then

$$
\int_{V(t)}\left[\rho(\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u)+\nabla p-\rho\mathbf g\right]dV=0.
$$

Since this holds for arbitrary material volumes and the fields are continuous, the integrand vanishes pointwise. Dividing by positive [density](../../../../density.md) gives the [Euler equations for an inviscid fluid](../../../../euler-equations-for-an-inviscid-fluid-split.md)

$$
\boxed{\partial_t\mathbf u+(\mathbf u\cdot\nabla)\mathbf u=-\rho^{-1}\nabla p+\mathbf g.}
$$

At a fixed physical time $t_0$, a [streamline](../../../../streamline.md) is a curve tangent to $\mathbf u(\cdot,t_0)$, which may be parametrized by $d\mathbf x/ds=\mathbf u(\mathbf x(s),t_0)$. The [chain rule](../../../../chain-rule.md) gives $d f(\mathbf x(s),t_0)/ds=\mathbf u\cdot\nabla f=0$, proving constancy along it. The time is held fixed; a time-dependent streamline statement does not by itself assert material conservation along particle trajectories.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [K](../../k.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
