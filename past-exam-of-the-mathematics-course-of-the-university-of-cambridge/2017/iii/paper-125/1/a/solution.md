<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonzero [isogeny of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md) $\phi:E_1\to E_2$, its [degree of an isogeny](../../../../../../degree-of-an-isogeny.md) is the degree of the induced extension of [function fields](../../../../../../function-field-of-an-algebraic-variety.md). Since $\phi$ commutes with negation, its first coordinate is a [rational function](../../../../../../rational-function.md) of $x_1$ alone. Write it in lowest terms as

$$
x_2(\phi(P))=R(x_1(P))=\frac{A(x_1(P))}{B(x_1(P))},\qquad\gcd(A,B)=1.
$$

The coordinate maps $x_i:E_i\to\mathbb P^1$ are [finite morphisms](../../../../../../finite-morphism.md) of degree two. Multiplying [function field](../../../../../../function-field-of-an-algebraic-variety.md) degrees in the commutative diagram $x_2\circ\phi=R\circ x_1$ gives the [degree of an isogeny from its x-coordinate map](../../../../../../degree-of-an-isogeny-from-its-x-coordinate-map.md):

$$
\boxed{\deg\phi=\max\{\deg A,\deg B\}.}
$$

This is the total degree, so the argument also covers an inseparable [isogeny of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md). Counting distinct points in the [kernel of an isogeny](../../../../../../kernel-of-an-isogeny.md) would give only its separable degree. The zero [group homomorphism](../../../../../../group-homomorphism.md) is assigned degree zero separately.

On a [Short Weierstrass form](../../../../../../short-weierstrass-form.md) $y^2=x^3+ax+b$ in [characteristic of a field](../../../../../../characteristic-of-a-field.md) other than two, the [elliptic-curve addition formula](../../../../../../elliptic-curve-addition-formula.md) gives

$$
x(2P)=\left(\frac{3x^2+a}{2y}\right)^2-2x
=\frac{x^4-2ax^2-8bx+a^2}{4(x^3+ax+b)}.
$$

There is no cancellation: at a root $r$ of $f(x)=x^3+ax+b$, the numerator equals $f'(r)^2$, which is nonzero because the [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) is nonzero. The numerator has degree four and the denominator degree three. Hence

$$
\boxed{\deg[2]=4.}
$$

For completeness, the same answer holds in characteristic two, where the displayed short equation is not a nonsingular model. On a general [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) use

$$
x(2P)=\frac{x^4-b_4x^2-2b_6x-b_8}{4x^3+b_2x^2+2b_4x+b_6},
$$

where $b_2=a_1^2+4a_2$, $b_4=a_1a_3+2a_4$, $b_6=a_3^2+4a_6$, and $b_8=a_1^2a_6+4a_2a_6-a_1a_3a_4+a_2a_3^2-a_4^2$. The [resultant](../../../../../../resultant.md) of this numerator and denominator is $\Delta^2$. Their resultant is therefore nonzero in every nonsingular case; even when the denominator drops degree, the numerator retains degree four.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
