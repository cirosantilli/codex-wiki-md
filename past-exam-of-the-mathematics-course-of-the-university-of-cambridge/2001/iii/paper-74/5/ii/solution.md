<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For [number fields](../../../../../../number-field.md), a [prime ideal](../../../../../../prime-ideal.md) divides the [different ideal](../../../../../../different-ideal.md) exactly when it is ramified. More precisely, the local [different exponent and tame ramification](../../../../../../different-exponent-and-tame-ramification.md) relation is $d_{\mathfrak P}\ge e_{\mathfrak P}-1$, with equality for tame ramification; if $e=1$, the finite residue extension is separable and the exponent is zero. One can see the ramification criterion directly from the [trace pairing](../../../../../../trace-pairing.md) modulo the base prime: when $e>1$ its quotient ring has a nonzero nilpotent ideal, whose elements pair to zero since multiplication by a nilpotent has trace zero. When $e=1$ the quotient is a product of finite separable fields and its trace pairing is nondegenerate. Its determinant is a unit exactly in the second case.

Let $M=K_1\cap K_2$. Any rational prime ramifying in $M$ must ramify in each $K_i$, because [ramification indices](../../../../../../ramification-index.md) multiply in a tower. It would then divide both [field discriminants](../../../../../../field-discriminant.md), contrary to their coprimality. Thus $M$ is unramified at every finite prime, so $|d_M|=1$. The [Minkowski lower bound for a number-field discriminant](../../../../../../minkowski-lower-bound-for-a-number-field-discriminant.md) excludes this for a field of degree $n>1$:

$$
\sqrt{|d_M|}\ge\left(\frac\pi4\right)^{r_2}\frac{n^n}{n!}>1.
$$

The last inequality follows already for the weakest signature bound $r_2\le n/2$: the expression starts above one at $n=2$ and increases with $n$. Consequently $M=\mathbb Q$.

For completeness, normality converts this intersection statement into the desired degree statement. Put $E=K_1K_2$. Restriction injects $\operatorname{Gal}(E/K_2)$ into $\operatorname{Gal}(K_1/\mathbb Q)$. The fixed field of its image in $K_1$ is exactly $K_1\cap K_2$, because $E/K_2$ is [Galois](../../../../../../finite-galois-extension.md). The [Galois correspondence](../../../../../../galois-correspondence.md) therefore gives $[E:K_2]=[K_1:M]=[K_1:\mathbb Q]$. This proves [coprime discriminants imply linear disjointness](../../../../../../coprime-discriminants-imply-linear-disjointness.md):

$$
\boxed{[K_1K_2:\mathbb Q]=[K_1:\mathbb Q][K_2:\mathbb Q].}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
