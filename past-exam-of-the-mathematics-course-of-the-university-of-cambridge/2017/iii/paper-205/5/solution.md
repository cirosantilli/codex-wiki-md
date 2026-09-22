<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $\lambda>0$ and labels $Y_i\in\{-1,1\}$, with squared-norm penalty normalized as $\lambda\alpha^TK\alpha$, the kernel [soft-margin support vector machine](../../../../../soft-margin-support-vector-machine.md) solves

$$
\boxed{\min_{\mu\in\mathbb R,\,\alpha\in\mathbb R^n}\left\{\frac1n\sum_{i=1}^n\bigl(1-Y_i(\mu+K_i^T\alpha)\bigr)_++\lambda\alpha^TK\alpha\right\}.}
$$

Here $(u)_+=\max(u,0)$ is the [hinge loss](../../../../../hinge-loss.md) building block, and $K_i$ is column $i$ of the symmetric [kernel matrix](../../../../../kernel-matrix.md). The prediction is

$$
\boxed{\widehat Y(x)=\operatorname{sgn}\left(\widehat\mu+\sum_i\widehat\alpha_i k(x,x_i)\right),}
$$

with a fixed class choice, for example $+1$, when the score is zero. Other positive rescalings of the penalty change numerical coefficients in the optimality equation but not the zero-coefficient conclusion.

For a finite [convex function](../../../../../convex-function.md) $f:\mathbb R^n\to\mathbb R$, its [subdifferential](../../../../../subdifferential.md) at $x$ is

$$
\partial f(x)=\{g\in\mathbb R^n:f(y)\ge f(x)+g^T(y-x)\text{ for every }y\in\mathbb R^n\}.
$$

For $f(x)=h(c^Tx+b)$, affine composition preserves the defining [convexity](../../../../../convex-function.md) inequality: for $0\le t\le1$,

$$
f(tx+(1-t)y)=h(t(c^Tx+b)+(1-t)(c^Ty+b))\le tf(x)+(1-t)f(y).
$$

If $v\in\partial h(u)$, the [subgradient inequality](../../../../../subgradient-inequality.md) gives $f(y)\ge f(x)+v c^T(y-x)$, proving $cv\in\partial f(x)$.

Conversely, let $g\in\partial f(x)$ and first suppose $c\ne0$. For every $z\in\ker c^T$, the [function](../../../../../function-split.md) is constant along $x+tz$. Applying the [subgradient inequality](../../../../../subgradient-inequality.md) for both signs of $t$ shows $g^Tz=0$. Thus $g$ is in the span of $c$, or $g=cv$ with $v=g^Tc/\|c\|_2^2$. Substituting $y=x+(a-u)c/\|c\|_2^2$ gives $h(a)\ge h(u)+v(a-u)$ for every real $a$. Hence $v\in\partial h(u)$. If $c=0$, $f$ is constant and $\partial f(x)=\{0\}$; since finite [convex](../../../../../convex-function.md) $h$ on all of $\mathbb R$ has a nonempty [subdifferential](../../../../../subdifferential.md) at $b$, $c\partial h(b)=\{0\}$ as well. This handles the case in which the suggested [orthogonal projection](../../../../../orthogonal-projection.md) would be undefined. Therefore

$$
\boxed{\partial f(x)=c\partial h(c^Tx+b).}
$$

This proves the [subdifferential under scalar affine composition](../../../../../subdifferential-under-scalar-affine-composition.md) identity with all its degenerate cases.

Let $m_i=Y_i(\widehat\mu+K_i^T\widehat\alpha)$ be a fitted [support-vector-machine margin](../../../../../support-vector-machine-margin.md). The [subdifferential](../../../../../subdifferential.md) of the [hinge loss](../../../../../hinge-loss.md) yields choices

$$
t_i=\begin{cases}1&m_i<1,\\{}[0,1]&m_i=1,\\0&m_i>1.\end{cases}
$$

Applying the affine-composition identity and the [subdifferential sum rule](../../../../../subdifferential-sum-rule.md) to the [convex](../../../../../convex-function.md) objective, its optimum satisfies

$$
2\lambda K\widehat\alpha=\frac1n\sum_iY_i t_iK_i,\qquad\sum_iY_it_i=0.
$$

The second equation is the intercept condition. Since $K$ is invertible, multiplying the first by $K^{-1}$ gives the [kernel support-vector coefficient from hinge activity](../../../../../kernel-support-vector-coefficient-from-hinge-activity.md) formula

$$
\widehat\alpha_i=\frac{Y_it_i}{2n\lambda}.
$$

In particular $\boxed{m_i>1\ \Longrightarrow\ \widehat\alpha_i=0.}$ Invertibility is needed for this statement about the chosen coefficients: for $K=\mathbf1\mathbf1^T$ with two positive labels, $\widehat\mu=2$ and $\widehat\alpha=(1,-1)^T$ give zero objective and both margins equal to two, while both coefficients are nonzero. A singular [kernel matrix](../../../../../kernel-matrix.md) allows coefficient changes in the [null space](../../../../../kernel-of-a-linear-map.md) without changing the fitted [function](../../../../../function-split.md).

At prediction time, the sum can omit all zero coefficients, requiring only the number of evaluations of the [positive-definite kernel](../../../../../positive-semidefinite-kernel.md) corresponding to retained [support vectors](../../../../../support-vector.md) rather than all $n$. This need not remove the cost of forming or solving with a dense training [kernel matrix](../../../../../kernel-matrix.md). Every misclassified point has $m_i\le0<1$, including a score-zero tie assigned to the opposite class, so $t_i=1$ and $\widehat\alpha_i=Y_i/(2n\lambda)\ne0$. Thus many classification errors imply many active [support vectors](../../../../../support-vector.md) and little prediction-time sparsity benefit. Correctly classified points inside the unit margin can also have nonzero coefficients; a point exactly on the margin need not have a nonzero coefficient.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
