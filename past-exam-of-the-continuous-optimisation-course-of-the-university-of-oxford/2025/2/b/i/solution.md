<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Taking the [natural logarithm](../../../../../natural-logarithm.md) of the positive product constraint gives $h(x)=\sum_i a_i\log x_i=0$. Its [gradient](../../../../../gradient.md) has entries $a_i/x_i>0$, so the equality [constraint qualification](../../../../../constraint-qualification.md) holds everywhere on the [feasible set](../../../../../feasible-region.md). Use the [optimization Lagrangian](../../../../../optimization-lagrangian.md)

$$
L(x,\lambda)=\sum_i a_ix_i-\lambda\sum_i a_i\log x_i.
$$

Stationarity requires $a_i-\lambda a_i/x_i=0$, so every $x_i=\lambda$. Substitution into the constraint, using $\sum_i a_i=1$, gives $\lambda=1$. Thus the only candidate for a [local minimum](../../../../../local-minimum.md) is $x=(1,\ldots,1)$.

To prove global minimality without assuming the inequality to be established, set $u_i=\log x_i$. The constraint becomes the [affine hyperplane](../../../../../affine-hyperplane.md) $\sum_i a_iu_i=0$, and the [objective function](../../../../../objective-function.md) becomes $F(u)=\sum_i a_ie^{u_i}$. Its [Hessian matrix](../../../../../hessian-matrix.md) $\operatorname{diag}(a_ie^{u_i})$ is [positive-definite](../../../../../positive-definite-bilinear-form.md), so $F$ is [strictly convex](../../../../../strictly-convex-function.md). The elementary tangent inequality $e^t\geq1+t$, with equality only at zero, gives

$$
F(u)\geq\sum_i a_i(1+u_i)=1.
$$

Equality forces every $u_i=0$. Therefore

$$
\boxed{x_*=(1,\ldots,1),\qquad\min\sum_i a_ix_i=1}.
$$

This point is the unique [global minimizer](../../../../../global-minimizer.md) and the only [local minimizer](../../../../../local-minimizer.md). The [logarithm](../../../../../logarithm.md) change of variables also explains why a multiplicative constraint leads to a [convex optimization](../../../../../convex-optimization-split.md) argument.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Continuous optimisation course of the University of Oxford](../../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
