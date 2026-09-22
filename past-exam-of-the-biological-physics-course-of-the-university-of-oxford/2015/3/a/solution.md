<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $e=q>0$ for the [elementary charge](../../../../elementary-charge.md) and $\epsilon=\epsilon_0\epsilon_r$ for the [permittivity](../../../../permittivity-split.md). Taking the bulk [electric potential](../../../../electric-potential.md) as zero, the [Boltzmann distribution](../../../../boltzmann-distribution.md) of point [ions](../../../../ion.md) gives $c_i(x)=c_i^\infty\exp[-ez_i\phi(x)/(k_BT)]$. Here $c_i$ is a [number density](../../../../number-density.md), not a molar [concentration](../../../../concentration.md). Combining this with [Poisson's equation](../../../../poisson-s-equation.md) gives the planar [Poisson-Boltzmann equation](../../../../poisson-boltzmann-equation.md)

$$
\phi''(x)=-\frac e\epsilon\sum_i z_ic_i^\infty e^{-ez_i\phi(x)/(k_BT)}.
$$

Multiplying by $\phi'$ and integrating from the neutral bulk, where $\phi=\phi'=0$, yields

$$
\frac\epsilon2(\phi')^2=k_BT\sum_i c_i^\infty\left(e^{-ez_i\phi/(k_BT)}-1\right).
$$

For the solution occupying $x>0$, with the field on the other side neglected, [Gauss's law](../../../../gauss-s-law.md) gives $\sigma=-\epsilon\phi'(0)$. On the branch that decays to zero without crossing it,

$$
\boxed{\sigma=\operatorname{sgn}(\phi_0)\sqrt{2\epsilon k_BT\sum_i c_i^\infty\left(e^{-ez_i\phi_0/(k_BT)}-1\right)}.}
$$

**Source sign qualification:** the unsigned square root printed in the paper gives $|\sigma|$. A negative wall [electric potential](../../../../electric-potential.md), such as the next part's $-73\,\mathrm{mV}$, has $\phi'(0)>0$ and hence $\sigma<0$, providing a concrete counterexample to interpreting that printed expression as signed [surface charge density](../../../../surface-charge-density.md). This is the planar [Grahame equation](../../../../grahame-equation.md), with an explicit sign convention.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
