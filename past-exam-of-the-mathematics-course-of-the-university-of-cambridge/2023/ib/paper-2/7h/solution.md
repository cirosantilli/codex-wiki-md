<h1 id="7h/solution">Solution</h1>

↑ **Parent:** [7H](../7h.md)

Use

$$
L(x,y,z,\lambda)
=x^2+y^4+z^6-\lambda(x+2y+3z-6).
$$

Stationarity gives

$$
2x=\lambda,
\qquad
4y^3=2\lambda,
\qquad
6z^5=3\lambda.
$$

Putting $t=\lambda/2$, this becomes

$$
x=t,\qquad y=t^{1/3},\qquad z=t^{1/5},
$$

and the constraint requires

$$
t+2t^{1/3}+3t^{1/5}=6.
$$

The left side is strictly increasing, and $t=1$ solves the equation. Hence

$$
\boxed{(x,y,z)=(1,1,1)},
\qquad
\boxed{f_{\min}=3},
\qquad
\lambda=2.
$$

The objective is convex and the constraint is affine. Its tangent-plane inequality at $(1,1,1)$ gives, for every feasible $(x,y,z)$,

$$
f(x,y,z)\geq3+(2,4,6)\cdot(x-1,y-1,z-1)=3,
$$

so the Lagrange point is globally optimal. Moreover, at the dual value $\lambda=2$, the infimum of the [Lagrangian function in constrained optimization](../../../../../lagrangian-function-in-constrained-optimization.md) is attained at the same point and equals three. The primal and dual values coincide, so strong duality holds.

For the value [function](../../../../../function-split.md), the multiplier convention above gives the [derivative of a constrained value function](../../../../../derivative-of-a-constrained-value-function.md)

$$
\phi'(b)=\lambda(b).
$$

At $b=6$, therefore,

$$
\boxed{\phi'(6)=2}.
$$

## ↑ Ancestors (10)

1. [7H](../7h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
