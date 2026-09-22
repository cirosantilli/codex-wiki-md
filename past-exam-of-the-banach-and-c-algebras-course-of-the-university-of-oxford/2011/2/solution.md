<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An element $a$ is a **[Normal element of a C-star algebra](../../../normal-element-of-a-c-star-algebra.md)** if $a^*a=aa^*$. It is a **[Unitary element of a C-star algebra](../../../unitary-element-of-a-c-star-algebra.md)** if $a^*a=aa^*=1$. Its [Banach algebra spectrum](../../../spectrum-of-an-element.md) is

$$
\boxed{\sigma_A(a)=\{z\in\mathbb C:a-z1\notin A^\times\},}
$$

where $A^\times$ is the [group of invertible elements of a Banach algebra](../../../group-of-invertible-elements-of-a-banach-algebra.md).

For normal $a$, the **[continuous functional calculus](../../../continuous-functional-calculus.md)** is the unique unital isometric star-isomorphism

$$
\Phi_a:C(\sigma_A(a))\longrightarrow C^*(1,a)\subseteq A,
\qquad f\longmapsto f(a),
$$

which sends the coordinate function $z\mapsto z$ to $a$. It preserves sums, products, complex [scalars](../../../scalar.md) and the involution: $\Phi_a(\overline f)=\Phi_a(f)^*$. In particular $\|f(a)\|=\max_{z\in\sigma_A(a)}|f(z)|$. The [spectral mapping theorem](../../../spectral-mapping-theorem.md) in this setting states

$$
\boxed{\sigma_A(f(a))=f(\sigma_A(a))\quad(f\in C(\sigma_A(a))).}
$$

The common unit and spectral permanence for C-star [subalgebras](../../../subalgebra.md) permit computing this spectrum in $A$ itself.

For unitary $u$, the C-star identity gives $\|u\|=\|u^*\|=1$. If $|z|>1$, $u-z1=-z(1-u/z)$ has a multiplicative inverse by the [Neumann series](../../../neumann-series.md). If $|z|<1$, write $u-z1=u(1-zu^*)$ and apply the same series. Therefore $\sigma_A(u)$ lies on the [unit circle](../../../complex-unit-circle.md).

For $|t|=1$, the denominator $1+\overline\lambda t$ is nonzero because $|\lambda|<1$. The function is consequently continuous on the spectrum, and

$$
|t+\lambda|^2=1+|\lambda|^2+\overline\lambda t+\lambda\overline t
=|1+\overline\lambda t|^2.
$$

Thus $|f(t)|=1$ throughout $\sigma_A(u)$, so $\overline f f=f\overline f=1$ there. Applying the star-homomorphism $\Phi_u$ proves

$$
\boxed{f(u)^*f(u)=f(u)f(u)^*=1.}
$$

Hence $f(u)$ is unitary. Explicitly, the same calculus gives

$$
\boxed{f(u)=(u+\lambda1)(1+\overline\lambda u)^{-1},}
$$

with the denominator's inverse also supplied by a norm-convergent Neumann series. This is the [Möbius transform of a unitary element](../../../mobius-transform-of-a-unitary-element.md). The conjugation on $\lambda$ in the denominator is essential to the unit-modulus identity.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2011](../../2011-split.md)
3. [Past exam of the Banach and C\*-algebras course of the University of Oxford](../../split.md)
4. [Banach and C\*-algebras course of the University of Oxford](../../../banach-and-c-algebras-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
