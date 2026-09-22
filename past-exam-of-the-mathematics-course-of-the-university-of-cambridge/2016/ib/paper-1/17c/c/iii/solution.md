<h1 id="17c/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\mathbf v$ denote the velocity relative to the uniformly rotating frame, and write $r_\perp^2=x^2+y^2$. For rotation $\boldsymbol\Omega=\Omega\mathbf e_z$, the [Euler equations for an inviscid fluid](../../../../../../../euler-equations-for-an-inviscid-fluid.md) in that frame are

$$
\partial_t\mathbf v+(\mathbf v\cdot\nabla)\mathbf v+2\boldsymbol\Omega\times\mathbf v=-\nabla\left(\frac p\rho+\Phi-\tfrac12\Omega^2r_\perp^2\right).
$$

The negative quadratic term is the [centrifugal potential](../../../../../../../centrifugal-potential.md), whose negative gradient is the outward [centrifugal acceleration](../../../../../../../centrifugal-acceleration.md) per unit mass. In [steady flow](../../../../../../../steady-flow.md), dotting the equation with $\mathbf v$ eliminates the [Coriolis force](../../../../../../../coriolis-force.md), since $\mathbf v\cdot(\boldsymbol\Omega\times\mathbf v)=0$. The remaining acceleration term is $\mathbf v\cdot\nabla(|\mathbf v|^2/2)$. Thus

$$
\mathbf v\cdot\nabla\left(\tfrac12|\mathbf v|^2+\frac p\rho+\Phi-\tfrac12\Omega^2r_\perp^2\right)=0.
$$

By part (b), **the [steady rotating-frame Bernoulli integral](../../../../../../../steady-rotating-frame-bernoulli-integral.md) is**

$$
\boxed{\tfrac12|\mathbf v|^2+\frac p\rho+\Phi-\tfrac12\Omega^2(x^2+y^2)=\text{constant on each relative streamline}.}
$$

Steadiness here is measured in the rotating frame, including the body-force potential used in that frame.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [17C](../../../17c.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ib](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
