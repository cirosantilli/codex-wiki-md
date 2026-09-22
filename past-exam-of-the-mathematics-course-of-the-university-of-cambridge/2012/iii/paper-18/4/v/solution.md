<h1 id="4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For the [curve generation criterion for an abelian variety](../../../../../../curve-generation-criterion-for-an-abelian-variety.md), first suppose $Y=X$ and an irreducible [Weil divisor](../../../../../../weil-divisor.md) $D$ avoids $C$. The preceding part gives $K(\mathcal O_X(D))=X$, so $\phi_{\mathcal O_X(D)}=0$ and $\mathcal O_X(D)\in\operatorname{Pic}^0(X)$. A nonzero [effective divisor](../../../../../../effective-cartier-divisor.md) cannot have this property: if $H$ is an [ample line bundle](../../../../../../ample-line-bundle.md) and $g=\dim X$, then the [intersection product of Cartier divisors](../../../../../../intersection-product-of-cartier-divisors.md) $D\cdot H^{g-1}$ is positive, whereas an algebraically trivial [line bundle](../../../../../../line-bundle.md) has zero intersection with every curve. The latter follows from constancy of degree along a connected family defining algebraic equivalence; the former is the positive projective degree of $D$ after replacing $H$ by a very ample power. This contradiction proves that $C$ meets every irreducible [Weil divisor](../../../../../../weil-divisor.md).

Conversely suppose $Y\ne X$. Fix $c_0\in C$, so $C\subseteq c_0+Y$. Use the permitted fiber theorem to choose a [morphism of varieties](../../../../../../morphism-of-algebraic-varieties.md) $f:X\to Z$ with $f^{-1}(z_0)=Y$. This morphism is nonconstant because $Y$ is proper. Choose an affine neighborhood $U$ of $z_0$. The irreducible image $f(X)$ has positive dimension, so its intersection with $U$ does too; some regular function $h$ on $U$ is nonconstant on this intersection. Then $F=h\circ f$ is a nonconstant rational function on $X$, regular on $f^{-1}(U)$.

The [pole divisor avoiding a fiber](../../../../../../pole-divisor-avoiding-a-fiber.md) construction applies: its pole [Weil divisor](../../../../../../weil-divisor.md) is nonzero. Indeed on the smooth, hence normal, [projective variety](../../../../../../projective-variety.md) $X$, a rational function with no codimension-one poles extends to a global regular function; every global regular function on a connected [projective variety](../../../../../../projective-variety.md) is constant. Every pole component $D_0$ lies outside $f^{-1}(U)$ and hence avoids $Y$. Therefore $D_0+c_0$ is an irreducible [Weil divisor](../../../../../../weil-divisor.md) disjoint from $c_0+Y$, and in particular from $C$. This proves the converse using precisely the fiber fact allowed in the question, without requiring a projective target $Z$. **The criterion is**

$$
\boxed{Y=X\quad\Longleftrightarrow\quad C\text{ meets every irreducible divisor of }X.}
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
