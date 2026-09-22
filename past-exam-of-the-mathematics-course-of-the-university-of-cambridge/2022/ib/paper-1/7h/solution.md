<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

Starting from $x_0\in\mathbb R^n$, [gradient descent](../../../../../gradient-descent.md) repeatedly computes the gradient and updates

$$
x_{k+1}=x_k-\eta\nabla f(x_k),
$$

stopping when the gradient norm, step, or objective decrease is sufficiently small.

The Hessian bounds say that $f$ is $\alpha$-[strongly convex](../../../../../strongly-convex-function.md) and has $\beta$-[smooth gradient](../../../../../lipschitz-gradient.md). With $\eta=1/\beta$,

$$
f(x_k)-f(x_*)
\leq
\left(1-\frac{\alpha}{\beta}\right)^k
\bigl(f(x_0)-f(x_*)\bigr).
$$

Thus the iteration count is

$$
O\left(\frac{\beta}{\alpha}\log\frac1\varepsilon\right);
$$

convergence becomes slower linearly with the [condition number](../../../../../condition-number.md) $\kappa=\beta/\alpha$.

For

$$
f(x,y,z)=x^2+100y^2+10000z^2,
$$

the [Hessian matrix](../../../../../hessian-matrix.md) is $\operatorname{diag}(2,200,20000)$, so

$$
\boxed{\kappa=10000}.
$$

Take

$$
\boxed{A=\operatorname{diag}(1,1/10,1/100)}.
$$

Then

$$
(f\circ A)(u,v,w)=u^2+v^2+w^2,
$$

whose Hessian is $2I$ and whose condition number is $1$.

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
