<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [subgradient inequality](../../../../subgradient-inequality.md) for the [differentiable](../../../../differentiable-function.md) [convex function](../../../../convex-function.md) $f$ gives

$$
\phi(u)=f(u)-f(y)-\nabla f(y)^T(u-y)\geq0\qquad\text{for every }u.
$$

Thus $y$ is a [global minimizer](../../../../global-minimizer.md) of $\phi$ with value zero. Subtracting an [affine function](../../../../affine-function.md) preserves [convexity](../../../../convex-function.md).

We must also justify using part (a) for $\phi$, since its [partial derivative](../../../../partial-derivative.md) can differ from that of $f$. First show that condition (6) for a singleton block implies the full coordinate [Lipschitz continuity](../../../../lipschitz-continuity.md) estimate

$$
|\partial_i f(z+te_i)-\partial_i f(z)|\leq L_i|t|,\qquad z\in\mathbb R^n,\ t\in\mathbb R.
$$

If $\partial_i f(z)\ne0$, choose $\alpha=-t/\partial_i f(z)$ in (6). If it is zero but $\partial_i f(z+te_i)\ne0$, apply the same argument starting at $z+te_i$ and reverse the displacement. If both [partial derivatives](../../../../partial-derivative.md) are zero, the estimate is immediate. The availability of all real $\alpha$ in (6) justifies these choices.

Now $\partial_i\phi(z)=\partial_i f(z)-\partial_i f(y)$, so differences of this [partial derivative](../../../../partial-derivative.md) along coordinate lines are unchanged. Hence $\phi$ has the same [coordinate Lipschitz continuity](../../../../coordinate-lipschitz-continuity.md) constant $L_i$ and satisfies the singleton version of (6). Apply part (a) to $\phi$ with [step size](../../../../step-size.md) $1/L_i$:

$$
\phi\left(x-\frac{\partial_i\phi(x)}{L_i}e_i\right)
\leq\phi(x)-\frac{[\partial_i\phi(x)]^2}{2L_i}.
$$

Combining with its already established nonnegativity proves

$$
\boxed{0\leq\phi\left(x-\frac{\partial_i\phi(x)}{L_i}e_i\right)\leq\phi(x)-\frac{[\partial_i\phi(x)]^2}{2L_i}.}
$$

**The coordinate estimate survives subtraction of the supporting [affine function](../../../../affine-function.md).** This is the step that allows the arbitrary comparison point $y$ to be exploited in part (c).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the optimisation for data science course of the University of Oxford](../../../split.md)
5. [Optimisation for data science course of the University of Oxford](../../../../optimisation-for-data-science-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
