<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On $V$, the [bilinear form](../../../../bilinear-form-split.md) $a$ is symmetric, and part (b) proves $a(v,v)\geq\alpha\|v\|_1^2$. Thus $a$ is an [inner product](../../../../inner-product-split.md): $a(v,v)\geq0$, and equality forces $v=0$. Its induced [energy norm](../../../../energy-norm.md) is $\|v\|_a=\sqrt{a(v,v)}$. For any real scalar $t$,

$$
\|tv\|_a=|t|\|v\|_a.
$$

The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) for this [inner product](../../../../inner-product-split.md) follows directly by expanding $a(p-tq,p-tq)\geq0$ and minimizing over $t$ when $q\ne0$. Hence

$$
\begin{aligned}
\|p+q\|_a^2
&=\|p\|_a^2+2a(p,q)+\|q\|_a^2\\
&\leq\bigl(\|p\|_a+\|q\|_a\bigr)^2,
\end{aligned}
$$

which proves the [triangle inequality](../../../../triangle-inequality.md). This verifies every [norm](../../../../norm.md) axiom. In fact, the estimates from part (b) give the [equivalent norms](../../../../equivalent-norms.md)

$$
\boxed{\sqrt\alpha\|v\|_1\leq\|v\|_a\leq\sqrt{2\mu+3\lambda}\|v\|_1.}
$$

Subtract the discrete [weak formulation](../../../../weak-formulation.md) from the continuous one to get [Galerkin orthogonality](../../../../galerkin-orthogonality.md),

$$
a(u-u_h,v_h)=0\qquad(v_h\in V_h).
$$

For any $v_h\in V_h$, write $u-v_h=(u-u_h)+(u_h-v_h)$. The second summand is in $V_h$, so expansion and [Galerkin orthogonality](../../../../galerkin-orthogonality.md) give the [Pythagorean theorem](../../../../pythagorean-theorem.md) in the [energy norm](../../../../energy-norm.md):

$$
\boxed{\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2.}
$$

The last term is nonnegative and vanishes exactly when $v_h=u_h$. Choosing $v_h=u_h$ attains the lower bound, proving

$$
\boxed{\|u-u_h\|_a=\min_{v_h\in V_h}\|u-v_h\|_a.}
$$

Thus $u_h$ is the unique [best approximation](../../../../best-approximation-in-a-normed-space.md); the map $u\mapsto u_h$ is the [orthogonal projector](../../../../orthogonal-projection.md) onto $V_h$ for the [linear elasticity](../../../../linear-elasticity.md) [energy norm](../../../../energy-norm.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the finite element methods for partial differential equations course of the University of Oxford](../../../split.md)
5. [Finite element methods for partial differential equations course of the University of Oxford](../../../../finite-element-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
