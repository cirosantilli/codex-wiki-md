<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For smooth [inviscid flow](../../../../../inviscid-flow.md) of constant [mass density](../../../../../density.md) under a conservative [body force](../../../../../body-force.md), [Kelvin's circulation theorem](../../../../../kelvin-s-circulation-theorem.md) states that the [circulation](../../../../../circulation-physics.md) around any closed [material curve](../../../../../material-curve.md) is conserved:

$$
\boxed{\frac{d\Gamma}{dt}=0.}
$$

The constant-[mass density](../../../../../density.md) assumption is the usual homogeneous [incompressible flow](../../../../../incompressible-flow.md) setting here. Merely requiring $\nabla\cdot\mathbf u=0$ in a fluid of varying [mass density](../../../../../density.md) would not by itself make the pressure term below a [gradient](../../../../../gradient.md).

Parameterize the [material curve](../../../../../material-curve.md) by a periodic particle label $s\in[0,1]$, writing $\mathbf r_t(s,t)=\mathbf u(\mathbf r(s,t),t)$. Differentiate its [line integral](../../../../../line-integral.md), keeping $s$ fixed:

$$
\begin{aligned}
\frac{d\Gamma}{dt}
&=\int_0^1\left[\frac{D\mathbf u}{Dt}\cdot\mathbf r_s+\mathbf u\cdot\partial_s\mathbf r_t\right]ds\\
&=\oint_{C(t)}\frac{D\mathbf u}{Dt}\cdot d\mathbf r+\int_0^1\partial_s\left(\frac12|\mathbf u|^2\right)ds\\
&=\oint_{C(t)}\frac{D\mathbf u}{Dt}\cdot d\mathbf r.
\end{aligned}
$$

The second term vanishes by periodicity. If the conservative [body force](../../../../../body-force.md) per unit [mass](../../../../../mass.md) is $-\nabla\Omega$, the [Euler momentum equation](../../../../../euler-equations-for-an-inviscid-fluid-split.md) gives

$$
\frac{D\mathbf u}{Dt}=-\frac1\rho\nabla p-\nabla\Omega=-\nabla(p/\rho+\Omega).
$$

Its [line integral](../../../../../line-integral.md) around a [closed curve](../../../../../closed-curve.md) is zero, proving the claim. The [velocity field](../../../../../velocity-field.md) must remain smooth on the moving curve, which cannot pass through a [line vortex](../../../../../line-vortex.md) singularity during this argument. No assumption of [irrotational flow](../../../../../irrotational-flow.md) was needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
