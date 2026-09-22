<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $z_i=(\mathbf x_i,\mathbf v_i)$ and $dz_i=d^3x_i\,d^3v_i$. Indistinguishability gives an [exchangeable](../../../../exchangeable-random-variables.md) ensemble. Define unit-normalized [marginal distributions](../../../../marginal-distribution.md)

$$
p_1(z_1,t)=\int\varrho\,dz_2\cdots dz_N,\qquad
p_2(z_1,z_2,t)=\int\varrho\,dz_3\cdots dz_N.
$$

Integrating the [dissipative Liouville equation](../../../../dissipative-liouville-equation.md) over $z_2,\ldots,z_N$ removes their boundary fluxes. The $N-1$ identical pair terms remain:

$$
\partial_tp_1+\mathbf v\cdot\nabla_{\mathbf x}p_1
+(N-1)\nabla_{\mathbf v}\cdot\int K(\mathbf x,\mathbf x_\star)(\mathbf v_\star-\mathbf v)p_2(z,z_\star,t)\,dz_\star=0.
$$

This is the first equation of a [BBGKY hierarchy](../../../../bbgky-hierarchy.md), with no independence assumed yet.

The additional physical assumption is a [mean-field closure for velocity alignment](../../../../mean-field-closure-for-velocity-alignment.md): neglect pair correlations, $p_2(z,z_\star,t)\simeq p_1(z,t)p_1(z_\star,t)$. Initial independence alone does not make this exact at later times, because the particles interact. In the usual number convention, $f=Np_1$ and the [two-particle distribution function](../../../../two-particle-distribution-function.md) is $f_2=N(N-1)p_2$. Consequently the closed equation at finite $N$ is

$$
\partial_tf+\mathbf v\cdot\nabla_{\mathbf x}f
+\left(1-\frac1N\right)\nabla_{\mathbf v}\cdot\bigl(f\mathbf L[f]\bigr)\simeq0,
\qquad
\mathbf L[f](z)=\int K(\mathbf x,\mathbf x_\star)(\mathbf v_\star-\mathbf v)f(z_\star,t)\,dz_\star.
$$

Neglecting the relative $1/N$ correction gives the intended [mean-field alignment equation](../../../../mean-field-alignment-equation.md):

$$
\boxed{\partial_tf+\mathbf v\cdot\nabla_{\mathbf x}f+\nabla_{\mathbf v}\cdot\bigl(f\mathbf L[f]\bigr)=0.}
$$

Equivalently, the closure $f_2\simeq ff_\star$ incorporates this large-$N$ approximation. It cannot be an exact finite-$N$ identity with $\int f=N$, since $\int f_2\,dz_\star=(N-1)f$ whereas $\int ff_\star\,dz_\star=Nf$.

There is also a consistent finite-$N$ convention yielding the boxed equation directly under the independence closure: define $\widetilde f=(N-1)p_1$ instead. Its total [normalization of a probability distribution](../../../../normalization-of-a-probability-distribution.md) is $N-1$, rather than the physical particle number $N$. Thus the displayed source equation needs a stated [normalization of a probability distribution](../../../../normalization-of-a-probability-distribution.md) convention, or the large-$N$ approximation, in addition to neglect of correlations. In the remaining parts we use the displayed [mean-field alignment equation](../../../../mean-field-alignment-equation.md) itself; its moment identities do not depend on the total [normalization of a probability distribution](../../../../normalization-of-a-probability-distribution.md).

## ↑ Ancestors (12)

1. [C](../c.md)
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
