<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Every [nonprincipal Dirichlet character](../../../../../../nonprincipal-dirichlet-character.md) modulo the [prime](../../../../../../prime-number.md) $q$ is primitive, so its finite [Fourier coefficients](../../../../../../fourier-coefficient.md) have modulus one off zero; the coefficient at zero is zero by [character orthogonality](../../../../../../character-orthogonality.md). [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) gives

$$
\sum_{M<n\le M+N}\chi(n)
=q^{-1/2}\sum_{a=1}^{q-1}\widehat\chi(a)\sum_{M<n\le M+N}e(an/q).
$$

The finite [geometric series](../../../../../../geometric-series.md) gives

$$
\left|\sum_{M<n\le M+N}e(an/q)\right|
\le\frac{2}{|1-e(a/q)|}\le C\|a/q\|_{\mathbb R/\mathbb Z}^{-1}.
$$

The printed hint omits $n$ from the exponential; its literal constant summand would not obey the bound for arbitrary $N$. The geometric-series calculation proves the needed estimate independently. Pairing $a$ with $q-a$ gives

$$
\left|\sum_{M<n\le M+N}\chi(n)\right|
\le C\sqrt q\,2\sum_{a=1}^{(q-1)/2}\frac1a
\ll\sqrt q\log q.
$$

The last sum is a [harmonic number](../../../../../../harmonic-number.md). This proves the [Pólya–Vinogradov inequality](../../../../../../polya-vinogradov-inequality.md) uniformly in $M$ and $N$; complete blocks of length $q$ also vanish by [Orthogonality of Dirichlet characters](../../../../../../orthogonality-of-dirichlet-characters.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
