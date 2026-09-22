<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [place of a number field](../../../../../place-of-a-number-field.md) is an equivalence class of nontrivial [absolute values on a field](../../../../../absolute-value-algebra.md). Its finite places correspond to nonzero prime ideals of the [ring of integers of a number field](../../../../../ring-of-integers.md); its infinite places come from real embeddings and conjugate pairs of complex embeddings.

For a [embedding of a number field into a p-adic algebraic closure](../../../../../embedding-of-a-number-field-into-a-p-adic-algebraic-closure.md) $\iota:K\hookrightarrow\overline{\mathbb Q}_p$, pull back the [p-adic absolute value](../../../../../p-adic-absolute-value.md). This gives a place above $p$. Every element of $\operatorname{Gal}(\overline{\mathbb Q}_p/\mathbb Q_p)$ preserves that absolute value, by uniqueness of its extension to each finite local extension, so equivalent embeddings give the same place.

Conversely, a place $v$ above $p$ gives a [completion of a number field at a prime ideal](../../../../../completion-of-a-number-field-at-a-prime-ideal.md) $K_v$, a finite extension of $\mathbb Q_p$. Embed it into $\overline{\mathbb Q}_p$ and restrict to $K$. If two embeddings give the same place, they extend to two $\mathbb Q_p$-embeddings of this same completion. They are conjugate under the absolute [Galois group](../../../../../galois-group.md): their finite separable images lie in a finite normal closure, and an isomorphism of such images extends to an automorphism of the algebraic closure. The completion really is the closure of the embedded $K$, since rational coefficients are dense in the $\mathbb Q_p$-span of a primitive element. Thus we obtain the [embedding orbit description of finite places](../../../../../embedding-orbit-description-of-finite-places.md):

$$
\boxed{\{v\mid p\}\ \longleftrightarrow\ \operatorname{Gal}(\overline{\mathbb Q}_p/\mathbb Q_p)\backslash\operatorname{Emb}(K,\overline{\mathbb Q}_p).}
$$

For the [product formula](../../../../../product-formula.md), use normalized local factors

$$
|x|_{\mathfrak p}=(N\mathfrak p)^{-\operatorname{ord}_{\mathfrak p}(x)},\qquad
|x|_v=|\sigma(x)|\text{ at a real place},\qquad
|x|_v=|\sigma(x)|^2\text{ at a complex place}.
$$

The squared modulus at a complex place counts its two embeddings. Equivalently one can use ordinary complex modulus and put exponent two in the product. These [normalized local factors for the product formula](../../../../../normalized-local-factors-for-the-product-formula.md) must be specified; arbitrary representatives of place classes would not satisfy the unweighted printed formula.

The fractional [principal ideal](../../../../../principal-ideal.md) $(x)$ has only finitely many nonzero prime exponents. Its [ideal norm](../../../../../ideal-norm.md) is $|N_{K/\mathbb Q}(x)|$: for integral $x$, multiplication by $x$ on an [integral basis](../../../../../integral-basis.md) has this determinant in absolute value, equal to the index of $(x)$ in $\mathcal O_K$; a quotient gives the fractional case. Hence the finite-place product is $|N_{K/\mathbb Q}(x)|^{-1}$. The infinite-place product is $|N_{K/\mathbb Q}(x)|$, by the embedding expression for the [field norm](../../../../../field-norm.md). Therefore **all but finitely many local factors are one**, and

$$
\boxed{\prod_v|x|_v=1.}
$$

Finally, let $\Delta_K\ne0$ be the integer [field discriminant](../../../../../field-discriminant.md), defined by the determinant of the [trace pairing](../../../../../trace-pairing.md) on an [integral basis](../../../../../integral-basis.md). If a rational prime $p$ ramifies, the algebra $\mathcal O_K/p\mathcal O_K$ has a nonzero nilpotent element: use [prime ideal factorization](../../../../../prime-ideal-factorization.md) and the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) to see a nonzero nilpotent in a factor $\mathcal O_K/\mathfrak p^e$ with $e>1$. If $y$ is nilpotent, multiplication by $yz$ is nilpotent for every $z$ in this commutative algebra, and therefore has trace zero. Thus $y$ is in the radical of its [trace pairing](../../../../../trace-pairing.md), making the reduced discriminant zero. We have proved the [discriminant obstruction to ramification](../../../../../discriminant-obstruction-to-ramification.md):

$$
p\text{ ramifies}\implies p\mid\Delta_K.
$$

Only finitely many rational primes divide this nonzero integer, so **only finitely many primes ramify**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
