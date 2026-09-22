<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For the convention above, after approximately minimizing $\Phi(\cdot,\lambda^{[k]},\mu_k)$, update

$$
\boxed{\lambda_i^{[k+1]}=
\max\left\{0,\lambda_i^{[k]}-\frac{g_i(x^{[k+1]})}{\mu_k}\right\}.}
$$

The exact shifted-residual identity is

$$
\min\{g_i(x^{[k+1]}),\mu_k\lambda_i^{[k]}\}
=\mu_k(\lambda_i^{[k]}-\lambda_i^{[k+1]}).
$$

If the constraint is violated, $g_i(x^{[k+1]})\leq0$, its left side is $\min\{g_i,0\}$, and replacing the new multiplier by its limiting value gives the printed local estimate

$$
\boxed{\min\{g_i(x^{[k+1]}),0\}
\approx\mu_k(\lambda_i^{[k]}-\lambda_i^*).}
$$

For arbitrary iterates, the precise unshifted statement includes the negative part:

$$
\boxed{\min\{g_i(x^{[k+1]}),0\}
=\mu_k\min\{\lambda_i^{[k]}-\lambda_i^{[k+1]},0\}.}
$$

Thus the printed estimate describes approach from the violated side; it is not a universal signed equality on the feasible side. This qualification follows directly from the projection in the update.

Its numerical significance is that the [constraint violation](../../../../constraint-violation.md) is controlled by $\mu_k$ times the multiplier error, rather than by $\mu_k$ alone. Once multipliers are accurate, high feasibility accuracy can be obtained with a moderate positive penalty parameter. This avoids forcing $1/\mu_k$ to become enormous and reduces the [ill-conditioning](../../../../condition-number.md) of the inner minimization. Inactive constraints eventually have zero multiplier and zero violation.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
