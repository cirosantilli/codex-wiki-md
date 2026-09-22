<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\Phi=\varphi_\varepsilon$ and let $\Phi^*$ denote its [convex conjugate](../../../../../../convex-conjugate.md). Its [Fenchel–Young gap](../../../../../../fenchel-young-gap.md)

$$
H(x,y)=\Phi(x)+\Phi^*(y)-x\cdot y
$$

is nonnegative by the [Fenchel–Young inequality](../../../../../../fenchel-young-inequality.md), and the hypothesis says $\int H\,d\pi_\varepsilon\leq\varepsilon$.

First justify the integrability needed for the certificate. Finite second [moments](../../../../../../moment.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) imply, for every [transport plan](../../../../../../transport-plan.md) $\pi$,

$$
\int|x\cdot y|\,d\pi\leq
\left(\int|x|^2\,d\mu\right)^{1/2}
\left(\int|y|^2\,d\nu\right)^{1/2}<\infty.
$$

Since $\Phi\in L^1(\mu)$ and $H\in L^1(\pi_\varepsilon)$, the identity $\Phi^*(y)=H(x,y)-\Phi(x)+x\cdot y$ proves $\Phi^*\in L^1(\nu)$ by the [marginal distribution](../../../../../../marginal-distribution.md) property. In particular, no subtraction of infinite integrals is being used.

Set

$$
u(x)=\tfrac12|x|^2-\Phi(x),\qquad
v(y)=\tfrac12|y|^2-\Phi^*(y),\qquad
D=\int u\,d\mu+\int v\,d\nu.
$$

These are integrable [Kantorovich potentials](../../../../../../kantorovich-potential.md). The [Fenchel–Young inequality](../../../../../../fenchel-young-inequality.md) gives $u(x)+v(y)\leq\tfrac12|x-y|^2$. More precisely, for every [transport plan](../../../../../../transport-plan.md) $\pi$,

$$
\mathbb K(\pi)=D+\int H\,d\pi\geq D,
\qquad\mathbb K(\pi_\varepsilon)=D+\int H\,d\pi_\varepsilon\leq D+\varepsilon.
$$

Taking the infimum in the first inequality therefore proves

$$
\boxed{\mathbb K(\pi_\varepsilon)\leq\inf_{\pi\in\Pi(\mu,\nu)}\mathbb K(\pi)+\varepsilon.}
$$

The factor $1/2$ in the quadratic cost is essential for this exact gap identity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
