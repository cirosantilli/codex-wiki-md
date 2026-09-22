<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix $x$, and write $p=x-\alpha G_\alpha(x)$ and $g=G_\alpha(x)$. The supplied [subgradient](../../../../subgradient.md) relation gives $v=v_\alpha\in\lambda\partial\psi(p)$ with $g=\nabla f(x)+v$. The evaluation point in $\nabla f$ is $x$, whereas $v$ is a [subgradient](../../../../subgradient.md) at the new point $p$.

Apply the [subgradient inequality](../../../../subgradient-inequality.md) at $p$, with comparison point $x$:

$$
\lambda\psi(p)-\lambda\psi(x)\leq v^T(p-x)=-\alpha v^Tg.
$$

The [descent lemma](../../../../descent-lemma.md) for the $L$-[Lipschitz gradient](../../../../lipschitz-gradient.md) of $f$ gives

$$
f(p)-f(x)\leq-\alpha\nabla f(x)^Tg+\frac{L\alpha^2}{2}\|g\|^2.
$$

Adding these estimates proves the stronger, explicit inequality

$$
\boxed{\phi(p)-\phi(x)\leq-\alpha\left(1-\frac{L\alpha}{2}\right)\|G_\alpha(x)\|^2.}
$$

In particular, the [objective function](../../../../objective-function.md) decreases for $0<\alpha<2/L$ whenever the [proximal gradient mapping](../../../../proximal-gradient-mapping.md) is nonzero.

To justify the requested [big O notation](../../../../big-o-notation.md), we must check that $g$, which depends on $\alpha$, stays bounded. Suppose $\partial(\lambda\psi)(x)$ is nonempty, and choose a fixed $w$ in this [subdifferential](../../../../subdifferential.md). This holds for a finite-valued [convex function](../../../../convex-function.md) on $\mathbb R^n$, including both [norms](../../../../norm.md) in parts (a) and (b). By [monotonicity of a convex subdifferential](../../../../monotonicity-of-a-convex-subdifferential.md),

$$
(v-w)^T(p-x)\geq0.
$$

Substituting $p-x=-\alpha g$ and $v=g-\nabla f(x)$, and then using the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md), yields

$$
\|g\|^2\leq(\nabla f(x)+w)^Tg\leq\|\nabla f(x)+w\|\,\|g\|.
$$

Thus $\|g\|\leq C_x:=\|\nabla f(x)+w\|$, uniformly in $\alpha>0$. This [local boundedness of the proximal gradient mapping](../../../../local-boundedness-of-the-proximal-gradient-mapping.md) makes the remainder at most $LC_x^2\alpha^2/2$, so

$$
\boxed{\phi(x-\alpha G_\alpha(x))-\phi(x)\leq-\alpha\|\nabla f(x)+v_\alpha\|^2+O(\alpha^2).}
$$

**No differentiability of $\psi$ is needed.** If an [proper extended-real function](../../../../proper-extended-real-function.md) is allowed as the [regularization](../../../../regularization.md) term, the [subdifferential](../../../../subdifferential.md) condition at $x$ is a qualification for this uniform remainder; the preceding explicit descent inequality remains the useful statement whenever its quantities are finite.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
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
