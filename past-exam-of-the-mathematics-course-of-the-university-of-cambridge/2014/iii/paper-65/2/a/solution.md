<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $z\in\mathbb R^m$ for the perturbation variable and $y\in\mathbb R^m$ for its dual variable. The full [Fenchel conjugate](../../../../../../convex-conjugate.md) is $f^*(v,y)=\sup_{x,z}(\langle v,x\rangle+\langle y,z\rangle-f(x,z))$. One signed-marginal convention is

$$
\boxed{\varphi(x)=f(x,0),\quad\psi(y)=-f^*(0,y),\quad
p(z)=\inf_xf(x,z),\quad q(v)=\sup_y[-f^*(v,y)].}
$$

The primal problem of [convex perturbation duality](../../../../../../convex-perturbation-duality.md) is $\inf_x\varphi(x)=p(0)$ and its dual problem of [convex perturbation duality](../../../../../../convex-perturbation-duality.md) is $\sup_y\psi(y)=q(0)$. The signed dual marginal $q$ is concave; some conventions instead use $-q$ as a convex marginal. The definitions above fix all signs. [Weak duality](../../../../../../weak-duality.md) follows from $f(x,0)+f^*(0,y)\geq0$. Also $p^*(y)=f^*(0,y)$, so $q(0)=p^{**}(0)$.

For a sufficient [strong duality](../../../../../../strong-duality.md) condition, assume $f$ is jointly proper convex, $p$ is proper with $p(0)$ finite, and $p$ is finite and continuous in a neighborhood of $0$. More generally $0\in\operatorname{ri}(\operatorname{dom}p)$ suffices in finite dimensions. A supporting [subgradient](../../../../../../subgradient.md) $y^*\in\partial p(0)$ then exists, and

$$
p(z)\geq p(0)+\langle y^*,z\rangle,
\qquad p^*(y^*)=-p(0),\qquad \psi(y^*)=p(0).
$$

Thus the dual is attained with no gap. This condition does not by itself assert attainment of the primal infimum; that needs an additional compactness or [coercivity](../../../../../../coercive-function.md) argument.

The same [subgradient](../../../../../../subgradient.md) describes [sensitivity analysis in convex perturbation duality](../../../../../../sensitivity-analysis-in-convex-perturbation-duality.md): $p(z)\geq p(0)+\langle y^*,z\rangle$ bounds the optimum's change under perturbation. When $p$ is finite convex near zero, its one-sided directional derivative is $p'(0;d)=\max_{y\in\partial p(0)}\langle y,d\rangle$. If $\partial p(0)=\{y^*\}$, then $p$ is differentiable there and

$$
\boxed{p(z)=p(0)+\langle y^*,z\rangle+o(\|z\|).}
$$

These conditions allow first-order sensitivity predictions; without differentiability the [subgradient](../../../../../../subgradient.md) set gives directional bounds. Multipliers can measure the value of relaxing constraints, quantify changes in noise tolerance, and guide parameter choice without resolving every perturbed problem. For the constraint convention in part (b), the noise-budget sensitivity is negative the nonnegative constraint multiplier.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
