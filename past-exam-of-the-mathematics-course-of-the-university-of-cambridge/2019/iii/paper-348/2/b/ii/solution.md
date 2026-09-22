<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Use the intended strong convexity bound** $\gamma^\top D^2\varphi(x)\gamma\geq\lambda|\gamma|^2$. The original PDF omits $|\gamma|^2$ on the right. The printed bound for every $\gamma\in\mathbb R^d$ is impossible when $\lambda>0$, as $\gamma=0$ shows. Equivalently, the intended bound is stated for unit vectors. The norm of $D^2\zeta$ is the [operator norm](../../../../../../../operator-norm.md) induced by the [Euclidean norm](../../../../../../../euclidean-norm.md), or any matrix [norm](../../../../../../../norm.md) that bounds it.

Set

$$
\boxed{\varphi_\varepsilon=\varphi+\varepsilon\zeta,\qquad T_\varepsilon=\nabla\varphi_\varepsilon.}
$$

This function is $C^2$, and its [Hessian matrix](../../../../../../../hessian-matrix.md) satisfies

$$
\begin{aligned}
\gamma^\top D^2\varphi_\varepsilon(x)\gamma
&=\gamma^\top D^2\varphi(x)\gamma+\varepsilon\gamma^\top D^2\zeta(x)\gamma\\
&\geq\bigl(\lambda-\varepsilon\|D^2\zeta(x)\|_{\mathrm{op}}\bigr)|\gamma|^2\geq0.
\end{aligned}
$$

Part (i) therefore proves that $\varphi_\varepsilon$ is a [convex function](../../../../../../../convex-function.md). The perturbation can use up the entire positive lower bound defining a [strongly convex function](../../../../../../../strongly-convex-function.md); only [convexity](../../../../../../../convex-function.md), rather than strict positivity of the [Hessian matrix](../../../../../../../hessian-matrix.md), is asserted.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 348](../../../../paper-348-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
