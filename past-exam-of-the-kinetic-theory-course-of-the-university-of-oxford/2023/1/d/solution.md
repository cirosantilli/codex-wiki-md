<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use $dz=d^3x\,d^3v$ and set

$$
\rho(\mathbf x,t)=\boxed{\int f(\mathbf x,\mathbf v,t)\,d^3v},\quad
\mathcal E=\frac12\int|\mathbf v|^2f\,dz,\quad
\mathcal H=\int f\log f\,dz.
$$

For unit particle [mass](../../../../mass.md), $\rho$ is both the [number density](../../../../number-density.md) and the [mass density](../../../../density.md) in the number convention of [c](../c.md). A fixed reference scale inside the [logarithm](../../../../logarithm.md) changes $\mathcal H$ by a constant multiple of the conserved total [mass](../../../../mass.md), leaving its derivative unchanged.

**Both prefactors in the source's part (d) need correction.** Multiplication of the [mean-field alignment equation](../../../../mean-field-alignment-equation.md) by $|\mathbf v|^2/2$ and [integration by parts](../../../../integration-by-parts.md) gives

$$
\dot{\mathcal E}=\int f\mathbf v\cdot\mathbf L[f]\,dz
=\iint K(\mathbf x,\mathbf x_\star)\mathbf v\cdot(\mathbf v_\star-\mathbf v)ff_\star\,dz\,dz_\star.
$$

Exchange $z$ and $z_\star$, use the [symmetry](../../../../symmetry-physics.md) of $K$, and average the two expressions:

$$
\boxed{\dot{\mathcal E}=-\frac12\iint K(\mathbf x,\mathbf x_\star)|\mathbf v_\star-\mathbf v|^2ff_\star\,dz\,dz_\star\leq0.}
$$

The printed right-hand side omits $1/2$. This corrected [velocity-alignment energy dissipation](../../../../velocity-alignment-energy-dissipation.md) agrees with the pair-counting calculation in [a](../a.md).

For [velocity-alignment entropy production](../../../../velocity-alignment-entropy-production.md), let $A(\mathbf x,t)=\int K(\mathbf x,\mathbf x_\star)\rho(\mathbf x_\star,t)\,d^3x_\star$. The [velocity-space divergence](../../../../velocity-space-divergence.md) is $\nabla_{\mathbf v}\cdot\mathbf L[f]=-3A$. Assuming $f>0$ and sufficient decay, [integration by parts](../../../../integration-by-parts.md) yields

$$
\begin{aligned}
\dot{\mathcal H}
&=-\int(1+\log f)\left[\mathbf v\cdot\nabla_{\mathbf x}f+\nabla_{\mathbf v}\cdot(f\mathbf L[f])\right]dz\\
&=\int\mathbf L[f]\cdot\nabla_{\mathbf v}f\,dz
=-\int f\nabla_{\mathbf v}\cdot\mathbf L[f]\,dz\\
&=\boxed{3\iint K(\mathbf x,\mathbf x_\star)\rho(\mathbf x,t)\rho(\mathbf x_\star,t)\,d^3x\,d^3x_\star\geq0.}
\end{aligned}
$$

The printed formula omits the factor $3$ from the three [velocity](../../../../velocity.md) components. In $d$ spatial [dimensions](../../../../dimension-vector-space.md), that factor would be $d$. Zeros of $f$ can be treated by a regularized [entropy](../../../../entropy-split.md) calculation when the required integrability holds.

A concrete smooth counterexample to both printed coefficients is $K\equiv1$ and $f(z,0)=g(\mathbf x)(2\pi)^{-3/2}e^{-|\mathbf v|^2/2}$, where $g$ is a positive normalized [Gaussian distribution](../../../../normal-distribution.md). The total [mass](../../../../mass.md) is one, the total [momentum](../../../../momentum-split.md) is zero, and $\mathbf L[f]=-\mathbf v$ initially. The [kinetic energy](../../../../kinetic-energy.md) derivative is $-\int |\mathbf v|^2f\,dz=-3$, whereas the printed formula gives $-6$. The [entropy functional](../../../../entropy-functional.md) derivative is $3$, whereas the printed formula gives $1$.

The signs describe cooling of relative [velocities](../../../../velocity.md) and contraction in [phase space](../../../../phase-space.md): $\mathcal H$ increases, so the fine-grained [Gibbs entropy](../../../../gibbs-entropy.md) $-\mathcal H$ decreases. These dissipative particle dynamics are not an isolated [Hamiltonian system](../../../../hamiltonian-system.md); there is no contradiction with [Liouville's theorem](../../../../liouville-theorem.md) or the [Boltzmann equation](../../../../boltzmann-equation-split.md)'s usual [entropy](../../../../entropy-split.md) increase. The microscopic mechanism removing [kinetic energy](../../../../kinetic-energy.md) is outside this alignment model.

## ↑ Ancestors (12)

1. [D](../d.md)
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
