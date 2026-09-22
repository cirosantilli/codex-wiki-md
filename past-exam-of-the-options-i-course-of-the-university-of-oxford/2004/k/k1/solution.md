<h1 id="k/k1/solution">Solution</h1>

↑ **Parent:** [K1](../k1.md)

For a [material volume](../../../../material-volume.md), [conservation of mass](../../../../mass-conservation.md) and the [Reynolds transport theorem](../../../../reynolds-transport-theorem.md) give $\rho_t+\nabla\cdot(\rho u)=0$. Constant material [density](../../../../density.md), or equivalently [incompressibility](../../../../incompressible-flow.md) with the stated constant initial [density](../../../../density.md), reduces this to $\nabla\cdot u=0$.

In an fluid undergoing [inviscid flow](../../../../inviscid-flow.md) the stress is the isotropic [pressure](../../../../pressure-split.md) stress $-pI$. [Momentum conservation](../../../../momentum-conservation.md) for a [material volume](../../../../material-volume.md) then gives

$$
\frac d{dt}\int_{V(t)}\rho u\,dV=-\int_{\partial V(t)}pn\,dS+\int_{V(t)}\rho g\,dV.
$$

Transport and the [divergence theorem](../../../../divergence-theorem.md) localize this to

$$
\boxed{\rho Du/Dt=-\nabla p+\rho g,\qquad D/Dt=\partial_t+u\cdot\nabla.}
$$

For a steady flow, $u_t=0$. For an [irrotational flow](../../../../irrotational-flow.md) the [vorticity](../../../../vorticity-split.md) is zero, so the supplied identity gives $(u\cdot\nabla)u=\nabla(|u|^2/2)$. Uniform downward gravity is $g=-\nabla(gz)$, and constant [density](../../../../density.md) permits pulling $1/\rho$ inside the [pressure](../../../../pressure-split.md) gradient. Therefore

$$
\boxed{\nabla\left(p/\rho+|u|^2/2+gz\right)=0.}
$$

The [Bernoulli invariant](../../../../bernoulli-invariant.md) is constant throughout each [connected](../../../../connected-space.md) fluid region. Without irrotationality the corresponding steady statement generally gives a constant only along each [streamline](../../../../streamline.md).

## ↑ Ancestors (12)

1. [K1](../k1.md)
2. [K](../../k.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
