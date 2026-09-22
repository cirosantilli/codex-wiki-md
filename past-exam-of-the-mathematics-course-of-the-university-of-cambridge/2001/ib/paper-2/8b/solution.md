<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

For a [bilinear form](../../../../../bilinear-form.md) $\phi$, define $F_\phi:V\to V^*$ by $F_\phi(v)(u)=\phi(u,v)$. Bilinearity makes $F_\phi(v)$ a linear functional and makes $F_\phi$ linear in $v$. Conversely, every linear $F:V\to V^*$ defines a bilinear form by $\phi_F(u,v)=F(v)(u)$. These constructions undo each other, giving the desired bijective correspondence.

For a [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md), $F_\phi$ has zero kernel and is an isomorphism because $V$ and its [dual space](../../../../../dual-space.md) have the same finite dimension. For the two forms, put

$$
\boxed{\alpha=F_{\phi_1}^{-1}F_{\phi_2}.}
$$

It is an isomorphism and satisfies $\phi_1(u,\alpha v)=F_{\phi_1}(\alpha v)(u)=F_{\phi_2}(v)(u)=\phi_2(u,v)$ for all $u,v$. This is the [representation of a bilinear form relative to a nondegenerate bilinear form](../../../../../representation-of-a-bilinear-form-relative-to-a-nondegenerate-bilinear-form.md).

If both forms are symmetric, then

$$
\phi_1(u,\alpha v)=\phi_2(u,v)=\phi_2(v,u)=\phi_1(v,\alpha u)=\phi_1(\alpha u,v).
$$

Nondegeneracy makes the adjoint with respect to $\phi_1$ unique; this equality proves **$\boxed{\alpha^\dagger=\alpha}$** in that bilinear-form sense. No positivity or Hermitian conjugation is assumed over the arbitrary field.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
