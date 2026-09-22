<h1 id="4c/solution">Solution</h1>

↑ **Parent:** [4C](../4c.md)

The convex [Legendre transform](../../../../../convex-conjugate.md), or [convex conjugate](../../../../../convex-conjugate.md), is

$$
\boxed{f^*(p)=\sup_{x\in\mathbb R^n}\{p^Tx-f(x)\}.}
$$

For a differentiable strictly [convex function](../../../../../convex-function.md), an attained maximum is characterized by $p=\nabla f(x)$, and then $f^*(p)=p^Tx-f(x)$ at that maximizing $x$.

For the [affine covariance of the convex conjugate](../../../../../affine-covariance-of-the-convex-conjugate.md), assume $\lambda>0$ and substitute $y=x-x_0$:

$$
\begin{aligned}
g^*(p)&=\sup_y\{p^T(y+x_0)-\lambda f(y)+\mu\}\\
&=p^Tx_0+\mu+\lambda\sup_y\{(p/\lambda)^Ty-f(y)\}.
\end{aligned}
$$

Hence

$$
\boxed{g^*(p)=\lambda f^*(p/\lambda)+p^Tx_0+\mu.}
$$

Positive scaling is necessary for this supremum definition, although the printed formula does not specify it. For example, $f(x)=x^2/2$ and $\lambda=-1$ give $g^*(p)=+\infty$, not the finite expression $-p^2/2$. If the transform is instead defined as a stationary value using a locally invertible gradient, the same algebraic identity holds for any $\lambda\ne0$: the critical-point relation is $p=\lambda\nabla f(y)$, and substitution of that stationary $y$ gives the displayed formula. That extension does not assert a supremum for negative scaling.

For the [positive-definite quadratic form](../../../../../positive-definite-quadratic-form.md), symmetry and positive [eigenvalues](../../../../../eigenvalue.md) of $A$ give

$$
p^Tx-\tfrac12x^TAx=\tfrac12p^TA^{-1}p-\tfrac12(x-A^{-1}p)^TA(x-A^{-1}p).
$$

The second term is nonpositive and vanishes exactly at $x=A^{-1}p$. Therefore

$$
\boxed{f^*(p)=\tfrac12p^TA^{-1}p.}
$$

## ↑ Ancestors (10)

1. [4C](../4c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
