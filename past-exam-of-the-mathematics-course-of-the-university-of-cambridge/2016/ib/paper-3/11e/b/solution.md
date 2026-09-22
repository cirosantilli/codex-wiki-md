<h1 id="11e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The polynomial $f(x)=x^5+2x+2$ satisfies the [Eisenstein criterion](../../../../../../eisenstein-criterion.md) at the prime two: every nonleading coefficient is divisible by two, and the constant coefficient is not divisible by four. Thus it is irreducible over $\mathbb Q$ and is the [minimal polynomial](../../../../../../minimal-polynomial.md) of every one of its roots. Part (a) gives

$$
\mathbb Z[\alpha]/(5)\cong\mathbb F_5[x]/(\overline f).
$$

But

$$
f(x)=(x-1)(x^4+x^3+x^2+x+3)+5.
$$

In the quotient, the two nonzero classes of $x-1$ and $x^4+x^3+x^2+x+3$ multiply to zero. They are nonzero because their nonzero representative degrees are less than five. The quotient is not an [integral domain](../../../../../../integral-domain.md), so **$(5)$ is not a [prime ideal](../../../../../../prime-ideal.md)**.

For [ring homomorphisms](../../../../../../ring-homomorphism.md) preserving the identity, an image $\beta$ of $\alpha$ in the [Gaussian integers](../../../../../../gaussian-integer.md) would satisfy $f(\beta)=0$. The [minimal polynomial](../../../../../../minimal-polynomial.md) of $\beta$ over $\mathbb Q$ would then be $f$, of degree five. This is impossible because $\beta\in\mathbb Q(i)$ has degree at most two. Thus **there is no unital homomorphism $\mathbb Z[\alpha]\to\mathbb Z[i]$**. If homomorphisms are instead allowed not to preserve the identity, the zero map exists; every nonzero homomorphism into this integral domain is unital, because the image of one is a nonzero idempotent and hence one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11E](../../11e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
