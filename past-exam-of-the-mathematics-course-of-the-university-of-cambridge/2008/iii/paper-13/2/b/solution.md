<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose an upper ellipticity bound $\Lambda<\infty$ for the symmetric coefficient matrix, possible because its entries are bounded. Then

$$
\lambda\|Du\|_2^2\leq Q(u,u)\leq\Lambda\|Du\|_2^2.
$$

The [Poincaré inequality](../../../../../../poincare-inequality.md) on a bounded open set for zero-boundary functions states $\|u\|_2\leq C_P\|Du\|_2$. Consequently

$$
\frac\lambda{1+C_P^2}\|u\|_{W^{1,2}}^2\leq Q(u,u)\leq\Lambda\|u\|_{W^{1,2}}^2.
$$

The symmetric positive [bilinear form](../../../../../../bilinear-form.md) $Q$ is therefore an [inner product](../../../../../../inner-product.md), and its square-root norm is equivalent to the usual [Sobolev norm](../../../../../../sobolev-norm.md). Its triangle inequality follows from the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) for that [inner product](../../../../../../inner-product.md). [completeness](../../../../../../completeness.md) of $W_0^{1,2}$ in its original norm makes it a [Hilbert space](../../../../../../hilbert-space-split.md) in the $Q$ norm as well.

The linear functional $\ell(v)=-\int fv$ is bounded, since

$$
|\ell(v)|\leq\|f\|_2\|v\|_2\leq C_P\lambda^{-1/2}\|f\|_2 Q(v,v)^{1/2}.
$$

The Hilbert-space [Riesz representation theorem](../../../../../../riesz-representation-theorem.md) states that every [bounded linear functional](../../../../../../continuous-linear-functional.md) is the [inner product](../../../../../../inner-product.md) with a unique element. Applied in the $Q$ [inner product](../../../../../../inner-product.md) it gives a unique $u$ with $Q(u,v)=\ell(v)$ for all $v$, which is precisely the weak-solution identity. Alternatively uniqueness follows directly by testing the difference of two solutions with itself: $Q(u_1-u_2,u_1-u_2)=0$. Thus $\boxed{\text{the zero-boundary problem has exactly one weak solution}}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
