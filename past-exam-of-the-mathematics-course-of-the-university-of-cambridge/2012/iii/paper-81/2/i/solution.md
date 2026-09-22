<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $e=e(\mathfrak q/\mathfrak p)$, $f=f(\mathfrak q/\mathfrak p)$ and $g$ for the number of primes above $\mathfrak p$. The [Galois group](../../../../../../galois-group.md) acts transitively on those primes, with stabilizer $D_{\mathfrak q}$. The [fundamental identity for prime decomposition](../../../../../../fundamental-identity-for-prime-decomposition.md) and the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) therefore give

$$
[F:K]=efg,\qquad |D_{\mathfrak q}|=[F:K]/g=ef.
$$

It remains to establish that the residue action has image of order $f$, rather than assume this in the desired equality.

Use the [decomposition group of a prime and local Galois group](../../../../../../decomposition-group-of-a-prime-and-local-galois-group.md) identification $D_{\mathfrak q}=\operatorname{Gal}(F_{\mathfrak q}/K_{\mathfrak p})$. A generator of the [finite field extension](../../../../../../finite-field-extension.md) $k_{\mathfrak q}/k_{\mathfrak p}$ has a separable monic [minimal polynomial of an algebraic element](../../../../../../minimal-polynomial-of-an-algebraic-element.md). Lift its coefficients to $\mathcal O_{K_{\mathfrak p}}$. The [Hensel lemma](../../../../../../hensel-s-lemma.md) lifts each of its distinct residue roots to $F_{\mathfrak q}$. One such lift has field degree at most $f$, while its residue generates the degree-$f$ [finite field extension](../../../../../../finite-field-extension.md), so its field degree is exactly $f$ and its [ramification index of a prime ideal](../../../../../../ramification-index-of-a-prime-ideal.md) is one. It therefore generates an [unramified extension](../../../../../../unramified-extension.md) of degree $f$, and sending it to each of the other lifts gives its $f$ embeddings. Because $F_{\mathfrak q}/K_{\mathfrak p}$ is a [Galois extension](../../../../../../finite-galois-extension.md), these embeddings extend to its automorphisms. Their reductions realize every automorphism of $k_{\mathfrak q}/k_{\mathfrak p}$. Thus the residue action is surjective, and

$$
\boxed{|I_{\mathfrak q}|=|D_{\mathfrak q}|/f=e.}
$$

Now let $G$ be cyclic of order $\ell^2$, and let $H=\operatorname{Gal}(F/L)$ be its unique subgroup of order $\ell$. In a tower of [Galois extensions](../../../../../../finite-galois-extension.md), inertia maps onto inertia in the intermediate extension. This also follows from the just-proved order formula: its image has order $e(F/K)/e(F/L)=e(L/K)$, using multiplicativity of the [ramification index of a prime ideal](../../../../../../ramification-index-of-a-prime-ideal.md) in a tower. If $\mathfrak p$ ramifies in $L/K$, this image in $G/H$ is nontrivial. Every proper subgroup of $G$ is contained in $H$, so inertia upstairs must be $G$. Hence

$$
\boxed{e(F/K)=\ell^2,\qquad \mathfrak p\text{ is totally ramified in }F/K.}
$$

The [fundamental identity for prime decomposition](../../../../../../fundamental-identity-for-prime-decomposition.md) then also forces a single prime above $\mathfrak p$ and [residue-field degree](../../../../../../residue-field-degree.md) one.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
