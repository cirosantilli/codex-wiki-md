<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume real bounded coefficients, with a principal part defining a [uniformly elliptic operator](../../../../../../uniformly-elliptic-operator.md), say $a^{ij}\xi_i\xi_j\geq\lambda|\xi|^2$ for some $\lambda>0$, and assume $c\leq0$. No smoothness of the boundary is needed for this classical [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md). Its conclusion is

$$
\boxed{\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\}.}
$$

If $c=0$, the zero may be omitted. Only the symmetric part of the principal coefficients contributes to the [Hessian matrix](../../../../../../hessian-matrix.md) contraction.

For a strict inequality $Lu>0$, a positive interior maximum is impossible: there $Du=0$, $D^2u$ is negative semidefinite, and $cu\leq0$, so $Lu\leq0$. To reduce the non-strict case to this one, let $q(x)=e^{\kappa x_1}$. Boundedness of $b^1,c$ permits choosing $\kappa$ so large that

$$
Lq=q\bigl(\kappa^2a^{11}+\kappa b^1+c\bigr)
\geq q\bigl(\lambda\kappa^2-\|b^1\|_\infty\kappa-\|c\|_\infty\bigr)>0.
$$

Thus $L(u+\varepsilon q)>0$. The preceding maximum argument and continuity on the compact closure give

$$
\sup_\Omega(u+\varepsilon q)\leq\max\{0,\sup_{\partial\Omega}(u+\varepsilon q)\}.
$$

Let $\varepsilon\downarrow0$; the exponential is bounded on the bounded domain. This is the [exponential perturbation proof of the weak maximum principle with drift](../../../../../../exponential-perturbation-proof-of-the-weak-maximum-principle-with-drift.md), with the zeroth-order term included. For $c=0$, any interior maximum, of either sign, is impossible for the perturbed function, giving the sharper boundary bound. The sign restriction on $c$ is essential: a positive first [Dirichlet Laplacian eigenfunction](../../../../../../dirichlet-laplacian-eigenfunction.md) violates the conclusion for $L=\Delta+\lambda_1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
