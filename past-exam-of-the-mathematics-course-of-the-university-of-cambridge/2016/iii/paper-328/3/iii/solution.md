<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\Omega$ be a bounded piecewise smooth domain, $f=u|_{\partial\Omega}$ and $q=\partial_nu$, with $n$ the outward [normal vector](../../../../../../normal-vector.md). Integrating the [divergence form](../../../../../../divergence-form.md) from part (i) and using the [divergence theorem](../../../../../../divergence-theorem.md) gives two [global relations for a linear boundary value problem](../../../../../../global-relation-for-a-linear-boundary-value-problem.md):

$$
\boxed{\mathcal G(\lambda)=\int_{\partial\Omega}(v_\lambda q-f\partial_nv_\lambda)\,ds=0,\qquad\widetilde{\mathcal G}(\lambda)=\int_{\partial\Omega}(\widetilde v_\lambda q-f\partial_n\widetilde v_\lambda)\,ds=0.}
$$

These [conjugate global relations for the modified Helmholtz equation](../../../../../../conjugate-global-relations-for-the-modified-helmholtz-equation.md) are identities between the prescribed [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) and its unknown [normal derivative](../../../../../../normal-derivative.md); neither is a pointwise boundary equation. Both hold for every nonzero [boundary spectral parameter](../../../../../../spectral-parameter-for-a-linear-boundary-value-problem.md) under the usual trace regularity assumptions.

If $u$ is real, its two boundary traces $f,q$ are real. Since $\widetilde v_\lambda=\overline{v_{\overline\lambda}}$ and the outward [normal vector](../../../../../../normal-vector.md) is real,

$$
\boxed{\widetilde{\mathcal G}(\lambda)=\overline{\mathcal G(\overline\lambda)}.}
$$

Thus apply [complex conjugation](../../../../../../complex-conjugation.md) to the first [global relation for a linear boundary value problem](../../../../../../global-relation-for-a-linear-boundary-value-problem.md), and replace its parameter by $\overline\lambda$, to get the second. For complex $u$, conjugation would also replace its traces by their conjugates, so that argument requires the stated reality assumption. There is also an algebraic redundancy in this particular parametrization: $\widetilde v_\lambda=v_{1/\lambda}$, hence $\widetilde{\mathcal G}(\lambda)=\mathcal G(1/\lambda)$ even for complex data. This does not change the requested conjugation identity.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 328](../../../paper-328-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
