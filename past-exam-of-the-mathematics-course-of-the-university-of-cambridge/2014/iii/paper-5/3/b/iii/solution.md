<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $v\in C_c^\infty(U)$, two [integrations by parts](../../../../../../../integration-by-parts.md) give the [clamped Hessian identity](../../../../../../../clamped-hessian-identity.md)

$$
\sum_{i,j}\int_U(\partial_{ij}v)^2=\sum_{i,j}\int_U(\partial_{ii}v)(\partial_{jj}v)=\int_U(\Delta v)^2.
$$

By density it remains valid on $H_0^2(U)$. Each $\partial_i v$ has zero integral, first for compactly supported [test functions](../../../../../../../test-function.md) and then by $H^2$ convergence. Applying the [Neumann-Poincare inequality](../../../../../../../poincare-wirtinger-inequality.md) to each $\partial_i v$ gives

$$
\|\nabla v\|_2^2\leq C_P\sum_{i,j}\|\partial_{ij}v\|_2^2=C_P\|\Delta v\|_2^2.
$$

The zero-boundary [Poincaré inequality](../../../../../../../poincare-inequality.md) also gives $\|v\|_2^2\leq C_D\|\nabla v\|_2^2$. Hence, using a full-Hessian equivalent $H^2$ [norm](../../../../../../../norm.md),

$$
\boxed{\|v\|_{H^2}^2\leq\bigl(1+C_P+C_DC_P\bigr)\|\Delta v\|_2^2\quad(v\in H_0^2(U)).}
$$

Thus $a(u,v)=\int_U\Delta u\Delta v$ is an [inner product](../../../../../../../inner-product.md) whose [norm](../../../../../../../norm.md) is equivalent to the complete $H^2$ [norm](../../../../../../../norm.md) on the [clamped second-order Sobolev space](../../../../../../../clamped-second-order-sobolev-space.md). The functional $L(v)=\int_Ufv$ is bounded for this [norm](../../../../../../../norm.md) by the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) and the displayed bound. Apply the [Riesz representation theorem](../../../../../../../riesz-representation-theorem.md), or the [Lax-Milgram theorem](../../../../../../../lax-milgram-theorem.md), to get a unique $u\in H_0^2(U)$ representing $L$. **The [clamped biharmonic problem](../../../../../../../clamped-biharmonic-problem.md) has a unique [weak solution](../../../../../../../weak-solution.md) for every $f\in L^2(U)$**, with $\|u\|_{H^2}\leq C\|f\|_2$ and no zero-integral compatibility condition.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
