<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [infinitesimal strain tensor](../../../../infinitesimal-strain-tensor.md) $\varepsilon(v)=\tfrac12(\nabla v+(\nabla v)^{\mathsf T})$ and the [divergence](../../../../divergence.md) are linear in $v$. Consequently the given $a$ is a [symmetric bilinear form](../../../../symmetric-bilinear-form.md), and

$$
a(v,v)=2\mu\|\varepsilon(v)\|_0^2+\lambda\|\operatorname{div}v\|_0^2\geq0.
$$

For a matrix-valued [function](../../../../function-split.md), $\|\cdot\|_0$ here uses the [Frobenius inner product](../../../../frobenius-inner-product.md) pointwise and then the [L2 norm](../../../../l2-norm.md). All expressions are finite for $v\in H^1(\Omega;\mathbb R^3)$.

Expand the quadratic term at $\theta v+(1-\theta)w$. The [linearity](../../../../linearity.md) of $\ell$ cancels its contribution to the difference, giving

$$
\begin{aligned}
\theta J(v)+(1-\theta)J(w)-J(\theta v+(1-\theta)w)
&=\frac{\theta(1-\theta)}2\bigl(a(v,v)-2a(v,w)+a(w,w)\bigr)\\
&=\frac{\theta(1-\theta)}2a(v-w,v-w)\\
&=\theta(1-\theta)\left(\mu\|\varepsilon(v-w)\|_0^2+\frac\lambda2\|\operatorname{div}(v-w)\|_0^2\right).
\end{aligned}
$$

For $0\leq\theta\leq1$, this is nonnegative. Therefore

$$
\boxed{J(\theta v+(1-\theta)w)\leq\theta J(v)+(1-\theta)J(w),}
$$

so $J$ is a [convex functional](../../../../convex-functional.md) on the whole [Sobolev space](../../../../sobolev-space-split.md). No boundary condition is needed for this conclusion. The argument uses nonnegativity of the quadratic term; uniqueness on the [zero-boundary Sobolev space](../../../../zero-boundary-sobolev-space.md) will instead use the [Korn inequality](../../../../korn-inequality.md) in part (b).

## ↑ Ancestors (12)

1. [A](../a.md)
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
