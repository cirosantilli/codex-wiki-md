<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [relativistic dust](../../../../../relativistic-dust.md), $p=0$, the [relativistic Euler equation](../../../../../relativistic-euler-equation.md) gives $\rho a_b=0$. The nowhere-vanishing [density](../../../../../density.md) therefore makes the [four-acceleration](../../../../../four-acceleration.md) zero: $u$ is a [timelike geodesic vector field](../../../../../timelike-geodesic-vector-field.md). Let $\alpha=u^\flat$ be the [differential one-form](../../../../../one-form.md) obtained by the [musical isomorphism](../../../../../musical-isomorphism.md). Its [exterior derivative](../../../../../exterior-derivative.md) satisfies

$$
(\iota_u d\alpha)_b=u^a(\nabla_a u_b-\nabla_bu_a)
=a_b-\frac12\nabla_b(u^au_a)=0.
$$

Here $\iota_u$ is the [interior product](../../../../../interior-product.md). By [hypersurface orthogonality](../../../../../hypersurface-orthogonality.md) and the [Frobenius theorem](../../../../../frobenius-theorem.md), $\alpha\wedge d\alpha=0$. Taking the [interior product](../../../../../interior-product.md) and using $\alpha(u)=-1$ gives

$$
0=\iota_u(\alpha\wedge d\alpha)
=-d\alpha-\alpha\wedge\iota_u d\alpha=-d\alpha.
$$

Thus $\boxed{du^\flat=0}$. By the [Poincaré lemma](../../../../../poincare-lemma.md), locally $\alpha=-dt$, and then $u(t)=-\alpha(u)=1$. Choose spatial [coordinate functions](../../../../../coordinate-function.md) $x^i$ on one level set of $t$ and extend them constantly along the [integral curves of a vector field](../../../../../integral-curve-of-a-vector-field.md) $u$, using its [smooth flow](../../../../../smooth-flow.md). This constructs $u=\partial_t$. Since $dt(\partial_i)=0$,

$$
g_{tt}=g(u,u)=-1,\qquad g_{ti}=\alpha(\partial_i)=-dt(\partial_i)=0.
$$

The metric on the orthogonal complement of a [timelike vector](../../../../../timelike-vector.md) is [positive-definite](../../../../../positive-definite-bilinear-form.md), so the [synchronous coordinates for irrotational dust](../../../../../synchronous-coordinates-for-irrotational-dust.md) have

$$
\boxed{u=\partial_t,\qquad g=-dt^2+g_{ij}(t,\mathbf x)\,dx^i\otimes dx^j.}
$$

This construction is local; crossing [geodesics](../../../../../geodesic.md) can prevent these [synchronous coordinates](../../../../../synchronous-coordinates.md) from covering a larger region.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the general relativity II course of the University of Oxford](../../../../split.md)
6. [General relativity II course of the University of Oxford](../../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
