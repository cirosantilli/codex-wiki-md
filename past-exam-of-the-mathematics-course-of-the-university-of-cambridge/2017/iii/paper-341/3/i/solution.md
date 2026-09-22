<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Dirichlet Laplacian eigenfunctions](../../../../../../dirichlet-laplacian-eigenfunction.md) and positive [Dirichlet Laplacian eigenvalues](../../../../../../dirichlet-laplacian-eigenvalue.md) on the interval of length two are

$$
\phi_j(x)=\sin\frac{j\pi(x+1)}2,\qquad
\lambda_j=\left(\frac{j\pi}{2}\right)^2,\qquad j\geq1.
$$

A [Sturm-Liouville eigenfunction expansion](../../../../../../sturm-liouville-eigenfunction-expansion.md) gives $u=\sum_jq_j(t)\phi_j$, with $q_j''+(\lambda_j-\alpha)q_j=0$. Thus all [normal modes](../../../../../../normal-mode.md) oscillate precisely when $\alpha<\lambda_1$.

To justify a spatially uniform bound for arbitrary appropriate data, assume the usual [wave equation](../../../../../../wave-equation-split.md) energy class $u(0)\in H_0^1(-1,1)$ and $u_t(0)\in L^2(-1,1)$, or smoother compatible data. The [energy method](../../../../../../energy-method.md) conserves

$$
E=\frac12\left(\|u_t\|_{L^2}^2+\|u_x\|_{L^2}^2-\alpha\|u\|_{L^2}^2\right).
$$

The sharp [Poincaré inequality](../../../../../../poincare-inequality.md) is $\|u\|_{L^2}^2\leq\lambda_1^{-1}\|u_x\|_{L^2}^2$. For $0\leq\alpha<\lambda_1$, this makes $E$ coercive with constant $1-\alpha/\lambda_1$; for $\alpha<0$, [coercivity](../../../../../../coercive-function.md) is immediate. The [one-dimensional Sobolev representative](../../../../../../one-dimensional-sobolev-representative.md) satisfies $|u(x,t)|\leq\sqrt2\,\|u_x(t)\|_{L^2}$ by the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). Hence the conserved [energy](../../../../../../energy.md) bounds $u$ uniformly in both variables.

At $\alpha=\lambda_1$, the smooth solution $u=t\phi_1$ is unbounded. At $\alpha>\lambda_1$, $u=e^{\sqrt{\alpha-\lambda_1}t}\phi_1$ is unbounded. Therefore

$$
\boxed{\alpha<\frac{\pi^2}{4}}.
$$

The bound depends on the initial data; it is not a single bound for all arbitrarily rescaled solutions. The energy-class hypothesis supplies pointwise meaning and excludes undefined rough-data interpretations.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
