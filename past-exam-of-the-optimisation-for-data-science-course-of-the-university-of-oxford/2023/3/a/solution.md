<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $x$ and put $g=\nabla_{\mathcal B}f(x)$, the [block coordinate gradient](../../../../block-coordinate-gradient.md). For $t\geq0$, define the one-variable [function](../../../../function-split.md) $q(t)=f(x-tg)$. By the [chain rule](../../../../chain-rule.md),

$$
q'(t)=-\nabla f(x-tg)^Tg=-\nabla_{\mathcal B}f(x-tg)^Tg.
$$

The last equality holds because the coordinates of $g$ outside $\mathcal B$ are zero. The [fundamental theorem of calculus](../../../../fundamental-theorem-of-calculus.md) and the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) therefore give

$$
\begin{aligned}
f(x-\alpha g)-f(x)
&=-\alpha\|g\|^2-\int_0^\alpha\big(\nabla_{\mathcal B}f(x-tg)-g\big)^Tg\,dt\\
&\leq-\alpha\|g\|^2+\int_0^\alpha\|\nabla_{\mathcal B}f(x-tg)-g\|\,\|g\|\,dt.
\end{aligned}
$$

For $\alpha\geq0$, the supplied condition (6), applied at the fixed starting point $x$ with parameter $t$, bounds the [integrand](../../../../integrand.md) by $L_{\mathcal B}t\|g\|^2$. Integration yields

$$
\boxed{f(x-\alpha\nabla_{\mathcal B}f(x))\leq f(x)-\alpha\left(1-\frac{L_{\mathcal B}\alpha}{2}\right)\|\nabla_{\mathcal B}f(x)\|^2.}
$$

This argument needs only the given directional [Lipschitz continuity](../../../../lipschitz-continuity.md) and continuous [differentiability](../../../../differentiability.md); [convexity](../../../../convex-function.md) is not needed for this part. If the [block coordinate gradient](../../../../block-coordinate-gradient.md) is zero, the inequality is equality.

## ↑ Ancestors (12)

1. [A](../a.md)
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
