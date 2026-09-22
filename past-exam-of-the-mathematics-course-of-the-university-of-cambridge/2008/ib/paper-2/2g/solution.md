<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

A complex number is an [algebraic number](../../../../../algebraic-number.md) over $\mathbb Q$ when it is a root of a nonzero rational polynomial. Its [minimal polynomial of an algebraic element](../../../../../minimal-polynomial-of-an-algebraic-element.md) is the unique monic polynomial in $\mathbb Q[X]$ of smallest degree annihilating it; polynomial division shows that it divides every rational polynomial annihilating the element, and it is irreducible.

Consider the surjective evaluation [ring homomorphism](../../../../../ring-homomorphism.md) $\operatorname{ev}_\alpha:\mathbb Z[X]\to\mathbb Z[\alpha]$. Certainly $(f)\subseteq\ker\operatorname{ev}_\alpha$. Because the nonconstant $f$ is irreducible over $\mathbb Z$, its content is a unit: otherwise its content and its nonconstant primitive part give a factorization into nonunits. By the [Gauss lemma for polynomials](../../../../../gauss-lemma-for-polynomials.md), $f$ is irreducible in $\mathbb Q[X]$ and is a scalar multiple of the minimal polynomial.

If $g\in\mathbb Z[X]$ vanishes at $\alpha$, then $f$ divides $g$ in $\mathbb Q[X]$. Primitive divisibility in [Gauss lemma for polynomials](../../../../../gauss-lemma-for-polynomials.md) implies division in $\mathbb Z[X]$ as well. Explicitly, write the rational quotient as $(a/b)h$ with $h$ primitive integral and $\gcd(a,b)=1$; the primitive product $fh$ shows that integrality of $(a/b)fh$ forces $b=1$. Thus the kernel is precisely $(f)$, and the [first isomorphism theorem for rings](../../../../../first-isomorphism-theorem-for-rings.md) yields

$$
\boxed{\mathbb Z[X]/(f)\cong\mathbb Z[\alpha],\qquad[g]\mapsto g(\alpha).}
$$

No monicity of $f$ is needed; this is an isomorphism of rings, not an assertion that either ring is a field.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
