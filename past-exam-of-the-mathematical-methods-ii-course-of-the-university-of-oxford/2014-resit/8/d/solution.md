<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The quadratic total [mechanical energy](../../../../mechanical-energy.md) is

$$
E=\frac12\dot{\boldsymbol\theta}^{\mathsf T}\mathbf T\dot{\boldsymbol\theta}+\frac12\boldsymbol\theta^{\mathsf T}\mathbf V\boldsymbol\theta,\qquad \frac{dE}{dt}=\dot{\boldsymbol\theta}^{\mathsf T}(\mathbf T\ddot{\boldsymbol\theta}+\mathbf V\boldsymbol\theta).
$$

For this frictionless conservative [double pendulum](../../../../double-pendulum.md), the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) for $L=K-U$ give

$$
\boxed{\mathbf T\ddot{\boldsymbol\theta}+\mathbf V\boldsymbol\theta=0,}
$$

or $8\ddot\theta_1+2\ddot\theta_2+(4g/l)\theta_1=0$ and $2\ddot\theta_1+\ddot\theta_2+(g/l)\theta_2=0$. Substitution immediately verifies [energy conservation](../../../../conservation-of-energy.md).

**Logical qualification.** [Energy conservation does not uniquely determine equations of motion](../../../../energy-conservation-does-not-uniquely-determine-equations-of-motion.md): the scalar equation $dE/dt=0$ alone does not determine both equations. For example, replacing their right side by $\mathbf G\dot{\boldsymbol\theta}$ with any nonzero antisymmetric matrix $\mathbf G$ preserves the same energy because $\dot{\boldsymbol\theta}^{\mathsf T}\mathbf G\dot{\boldsymbol\theta}=0$, while changing the dynamics. Such a gyroscopic force is absent from the specified pendulum. The conservative-force structure, supplied here by the [Lagrangian](../../../../lagrangian.md), is the additional information needed to justify the displayed equations rather than infer two independent equations from one scalar identity.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [2014 resit](../../../2014-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
