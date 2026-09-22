<h1 id="2/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Set $r^k=Ax^k-c$. Completing the square in the $y$-minimization gives

$$
\|y+r^k\|_2^2+\frac1{2\tau}\|y-y^k\|_2^2
=\frac{1+2\tau}{2\tau}\left\|y-\frac{y^k-2\tau r^k}{1+2\tau}\right\|_2^2+\text{a term independent of }y.
$$

Thus, with $\sigma=\tau/(1+2\tau)$, the steps in terms of the [proximal map](../../../../../../proximal-operator.md) of $\phi$ are

$$
\boxed{y^{k+1}=\operatorname{prox}_{\sigma\phi}\left(\frac{y^k+2\tau(c-Ax^k)}{1+2\tau}\right),\qquad
x^{k+1}=x^k-2\tau A^T(Ax^k+y^{k+1}-c)}.
$$

The factor $2$ comes from the squared residual without a $1/2$ prefactor. The [proximal map](../../../../../../proximal-operator.md) can equivalently be denoted $(I+\sigma\partial\phi)^{-1}$. Since $\phi$ is a finite [convex function](../../../../../../convex-function.md), it is continuous, and the quadratic makes the proximal minimizer unique.

A general convex $\phi$ may be nondifferentiable, so this last example need not satisfy the full $L$-smooth hypothesis of the preceding part. The formulas nevertheless remain well-defined: only the $x$ derivative is used explicitly. If $\phi$ has an $L_\phi$-[Lipschitz gradient](../../../../../../lipschitz-gradient.md), one may take $L=2(\|A\|_2^2+1)+L_\phi$ in the smooth proof, where $\|A\|_2$ is the [operator norm](../../../../../../operator-norm.md).

There is also a useful nonsmooth extension. Put $h(x,y)=\|Ax+y-c\|_2^2$, whose [Lipschitz gradient](../../../../../../lipschitz-gradient.md) constant is $L_h=2(\|A\|_2^2+1)$. For two updates, retain the mixed-point differences $(p,q)$ above, let $(a,b)=\nabla h(w)-\nabla h(\widetilde w)$, and let $d$ be the difference of the two selected [subgradients](../../../../../../subgradient.md) of $\phi$ at $y^+,\widetilde y^+$. The input difference is $(p,q+\tau(b+d))$ and the output difference is $(p-\tau a,q)$. Monotonicity of $\partial\phi$ gives $\langle q,d\rangle\geq0$. The same norm expansion now yields

$$
\|Tz-T\widetilde z\|_2^2
\leq\|z-\widetilde z\|_2^2
-\left(\frac{2\tau}{L_h}-\tau^2\right)\|a\|_2^2
-\frac{2\tau}{L_h}\|b\|_2^2-\tau^2\|b+d\|_2^2.
$$

For $0<\tau L_h\leq1$, discard the nonpositive $b$ term and use $2\tau/L_h-\tau^2\geq\tau^2$. The result is the [firmly nonexpansive mapping](../../../../../../firmly-nonexpansive-mapping.md) inequality for the full residual $\tau(a,b+d)$. Fixed points satisfy $\nabla_xh=0$ and $0\in\nabla_yh+\partial\phi$, exactly the [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md) for the convex objective. Thus the stated algorithm also converges for nonsmooth $\phi$ under this sufficient step bound, provided a minimizer exists; this extension uses monotonicity, not an unavailable gradient of $\phi$.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [2](../../2.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
