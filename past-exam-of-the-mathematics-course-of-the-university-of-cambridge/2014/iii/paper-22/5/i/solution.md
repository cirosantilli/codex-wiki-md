<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work in characteristic different from two, as in the number-field application below. Nonsingularity is equivalent to $b(a^2-4b)\ne0$. The chord through $P=(x,y)$ and $T=(0,0)$ has slope $y/x$. Using $y^2/x^2=x+a+b/x$ in the [elliptic-curve addition formula](../../../../../../elliptic-curve-addition-formula.md) gives

$$
\boxed{x^{\prime}=\frac b x,\qquad y^{\prime}=-\frac{by}{x^2}.}
$$

These formulas hold for $P\ne O,T$; addition interchanges $O$ and $T$.

It follows that $\xi=x+a+b/x=y^2/x^2$ and $\eta=y(1-b/x^2)$. The relation is

$$
\boxed{\eta^2=\xi\bigl(\xi^2-2a\xi+a^2-4b\bigr).}
$$

For a direct verification, observe that

$$
(\xi-a)^2-4b=(x-b/x)^2,
\qquad
\eta^2=\frac{y^2}{x^2}(x-b/x)^2.
$$

Therefore the [two-isogeny formula](../../../../../../two-isogeny-formula.md) is

$$
\boxed{\begin{aligned}
E^{\prime}&:Y^2=X(X^2-2aX+a^2-4b),\\
\phi(x,y)&=\left(x+a+\frac b x,\ y\left(1-\frac b{x^2}\right)\right),\\
\phi(O)&=\phi(T)=O.
\end{aligned}}
$$

The target [elliptic curve](../../../../../../elliptic-curve.md) is nonsingular because its corresponding coefficient product is $16b(a^2-4b)\ne0$. The [rational map of projective varieties](../../../../../../rational-map-of-projective-varieties.md) extends over the exceptional points to a morphism of smooth projective [algebraic curves](../../../../../../algebraic-curve.md); at both $O$ and $T$ its affine coordinates tend to infinity, giving the displayed values. A nonconstant morphism between [elliptic curves](../../../../../../elliptic-curve.md) sending $O$ to $O$ is a [group homomorphism](../../../../../../group-homomorphism.md), so this is an [isogeny of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md).

One can also see the quotient directly: translation by $T$ leaves $\xi,\eta$ invariant. The equation $x^2+(a-\xi)x+b=0$ makes the source [function field](../../../../../../function-field-of-an-algebraic-variety.md) a degree-two extension of the target [function field](../../../../../../function-field-of-an-algebraic-variety.md); its nontrivial automorphism is translation by $T$. Equivalently, the [degree of an isogeny from its x-coordinate map](../../../../../../degree-of-an-isogeny-from-its-x-coordinate-map.md) is two. The [kernel of an isogeny](../../../../../../kernel-of-an-isogeny.md) is precisely $\{O,T\}$. **Thus $\phi$ is a separable isogeny of degree two.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
