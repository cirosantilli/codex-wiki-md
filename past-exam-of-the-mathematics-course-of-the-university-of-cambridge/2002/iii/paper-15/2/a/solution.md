<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [multiplicative algebraic group](../../../../../../multiplicative-algebraic-group.md) $\mathbb G_m$ has [coordinate ring](../../../../../../coordinate-ring.md) $\mathbb C[t,t^{-1}]$. An algebraic morphism $f:\mathbb G_m\to\mathbb G_m$ therefore sends the invertible coordinate on the target to a [unit](../../../../../../unit-in-a-ring.md) of this [Laurent polynomial ring](../../../../../../laurent-polynomial-ring.md).

Every unit of $\mathbb C[t,t^{-1}]$ has the form $ct^i$, with $c\in\mathbb C^*$ and $i\in\mathbb Z$. To prove this, suppose Laurent polynomials $P,Q$ satisfy $PQ=1$. Write their least and greatest active exponents as $a\le b$ and $c\le d$. The least and greatest exponents in their product are $a+c$ and $b+d$, since their endpoint coefficients are nonzero. Both must be zero. Consequently

$$
(b-a)+(d-c)=0,
$$

so each factor has only one active exponent. This proves the asserted unit description.

Thus $f(t)=ct^i$. A [group homomorphism](../../../../../../group-homomorphism.md) sends the identity to the identity, so $f(1)=1$ and $c=1$. Conversely, for every integer $i$, including negative integers and zero, $t\mapsto t^i$ is regular on $\mathbb G_m$ and satisfies $(st)^i=s^it^i$. We obtain

$$
\boxed{\operatorname{Hom}_{\mathrm{alg.grp}}(\mathbb G_m,\mathbb G_m)=\{t\mapsto t^i:i\in\mathbb Z\}.}
$$

These are exactly the [characters of an algebraic torus](../../../../../../algebraic-torus-character.md) in the one-dimensional case. The algebraic-morphism requirement is essential to the argument: the map must come from the Laurent coordinate ring.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
