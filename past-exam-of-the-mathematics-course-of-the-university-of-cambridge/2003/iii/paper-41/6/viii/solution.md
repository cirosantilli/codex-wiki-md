<h1 id="6/viii/solution">Solution</h1>

↑ **Parent:** [Viii](../viii.md)

A [curved exponential family](../../../../../../curved-exponential-family.md) restricts a higher-dimensional full canonical family to a lower-dimensional smooth parameter surface:

$$
f(x;\theta)=h(x)\exp\{\eta(\theta)^\top t(x)-A(\eta(\theta))\},\qquad\theta\in\mathbb R^q,\quad\eta(\theta)\in\mathbb R^p,\quad q<p.
$$

The derivative matrix $J(\theta)=\partial\eta/\partial\theta$ has rank $q$. A genuinely curved surface is not merely an affine subfamily under a choice of natural coordinates. With $n$ iid observations the ambient sufficient statistic is $T_n=\sum_i t(X_i)$, and the parameter score and information are

$$
U_\theta=J(\theta)^\top[T_n-n\nabla A(\eta(\theta))],\qquad I_\theta=nJ(\theta)^\top\nabla^2A(\eta(\theta))J(\theta).
$$

The second-derivative terms from $\eta(\theta)$ have zero expectation because the centered sufficient statistic has mean zero. Under regularity, the constrained MLE is still first-order asymptotically normal with this information. Curvature affects higher-order bias, likelihood geometry and efficiency; concavity of the ambient likelihood need not survive along the nonlinear parameter surface.

For example, $N(\mu,\mu^2)$ with $\mu>0$ has $t(x)=(x,x^2)$ and natural parameters $\eta_1=1/\mu$, $\eta_2=-1/(2\mu^2)$, constrained by $\eta_2=-\eta_1^2/2$. It has one free parameter but generally still needs both $\sum X_i$ and $\sum X_i^2$ as sufficient statistics. To see why, a likelihood ratio between two samples is constant in $\mu$ only if their statistic differences satisfy $\Delta T_1/\mu-\Delta T_2/(2\mu^2)=\text{constant}$ for all positive $\mu$, forcing both differences to zero. Lower parameter dimension therefore does not generally reduce the minimal sufficient statistic to that dimension.

## ↑ Ancestors (11)

1. [Viii](../viii.md)
2. [6](../../6.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
