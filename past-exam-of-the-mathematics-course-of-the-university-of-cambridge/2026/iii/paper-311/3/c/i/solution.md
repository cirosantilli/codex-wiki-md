<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\Sigma_t$ be a [Cauchy hypersurface](../../../../../../../cauchy-surface.md) with induced metric $h_{ij}$, lapse $N$, shift $N^i$, and future unit normal $n^a$. For the normalization of the action in the question, the canonical momentum density is

$$
\Pi=2\sqrt h\,n^a\nabla_a\Phi
=\frac{2\sqrt h}{N}(\dot\Phi-N^i\partial_i\Phi).
$$

The equal-time [canonical commutation relations](../../../../../../../canonical-commutation-relation.md) are

$$
[\widehat\Phi(t,\mathbf x),\widehat\Phi(t,\mathbf y)]=0,
\qquad
[\widehat\Pi(t,\mathbf x),\widehat\Pi(t,\mathbf y)]=0,
$$

and

$$
\boxed{[\widehat\Phi(t,\mathbf x),\widehat\Pi(t,\mathbf y)]
=i\delta^{(3)}(\mathbf x-\mathbf y)}.
$$

With the conventional extra factor $1/2$ in the action, $\Pi$ loses the factor two.

For complex classical solutions, the [Klein-Gordon inner product](../../../../../../../klein-gordon-inner-product.md) is

$$
(\phi_1,\phi_2)_{KG}
=i\int_{\Sigma_t}d\Sigma^a
(\phi_1^*\nabla_a\phi_2-\phi_2\nabla_a\phi_1^*).
$$

The integrand is a conserved current because both fields obey the [Klein-Gordon equation](../../../../../../../klein-gordon-equation.md). Applying the [divergence theorem](../../../../../../../divergence-theorem.md) between two Cauchy hypersurfaces shows that the value is independent of the foliation, provided there is no boundary flux.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 311](../../../../paper-311-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
