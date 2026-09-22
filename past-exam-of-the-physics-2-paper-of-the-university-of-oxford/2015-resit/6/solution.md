<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For an ideal [inductor](../../../inductor.md) of constant [self-inductance](../../../self-inductance.md) $L$, the passive-sign [electric potential difference](../../../electric-potential-difference.md) is $V_L=L\,dI/dt$. The supplied [power](../../../power.md) is $V_LI$, so increasing the [electric current](../../../electric-current.md) quasistatically from zero stores

$$
U=\int V_LI\,dt=\int_0^I LI'\,dI'=\boxed{\frac12LI^2}.
$$

Any [electrical resistance](../../../electrical-resistance.md) would additionally dissipate [energy](../../../energy-split.md) as heat; it is not included in this stored magnetic [energy](../../../energy-split.md).

For a long vacuum [solenoid](../../../solenoid.md) with $N$ turns, axial length $\ell$ and cross-sectional area $A$, [Ampère's law](../../../ampere-s-circuital-law.md) gives $B=\mu_0(N/\ell)I$. Its [flux](../../../flux.md) linkage is $N\Phi=N BA$, so

$$
L=\frac{N\Phi}{I}=\frac{\mu_0N^2A}{\ell}.
$$

The nearly uniform field occupies volume $A\ell$, with negligible external-field [energy](../../../energy-split.md) in the long-solenoid approximation. Dividing its stored [energy](../../../energy-split.md) by this volume yields

$$
\boxed{u_B=\frac{U}{A\ell}=\frac12\mu_0\left(\frac N\ell\right)^2I^2=\frac{B^2}{2\mu_0}}.
$$

The vacuum and linear-inductance assumptions matter; a nonlinear magnetic material requires the appropriate field-energy integral rather than simply substituting a varying [inductance](../../../inductance.md) into $LI^2/2$.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2015 resit](../../2015-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
