<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [decomposition group](../../../../../../decomposition-group.md) of the chosen prime is its stabilizer under the [Galois group](../../../../../../galois-group.md):

$$
\boxed{D=D_{\mathfrak P\mid\mathfrak p}=\{\sigma\in G:\sigma(\mathfrak P)=\mathfrak P\}.}
$$

The [transitivity of the Galois action on primes](../../../../../../transitivity-of-the-galois-action-on-primes.md) identifies the primes of $M$ above $\mathfrak p$ with $G/D$ through $gD\mapsto g\mathfrak P$.

Put $H=\operatorname{Gal}(M/L)$. Contraction of prime ideals to $\mathcal O_L$ is constant on every $H$-orbit, because every element of $H$ fixes $L$ pointwise. It is surjective onto the primes of $L$ above $\mathfrak p$, since prime ideals extend in the integral extension $\mathcal O_M/\mathcal O_L$. Moreover, two primes of $M$ contracting to the same prime of $L$ are conjugate by $H$: the extension $M/L$ is Galois and the same transitivity theorem applies to it.

Thus the fibers of contraction are exactly the $H$-orbits on $G/D$. These orbits are the [double cosets](../../../../../../double-coset.md) $H\backslash G/D$, proving the [primes in an intermediate field as double cosets](../../../../../../primes-in-an-intermediate-field-as-double-cosets.md) correspondence

$$
\boxed{H\backslash G/D\xrightarrow{\sim}\{\mathfrak q\subset\mathcal O_L:\mathfrak q\mid\mathfrak p\},\qquad
HgD\longmapsto g\mathfrak P\cap\mathcal O_L.}
$$

Explicitly, replacing $g$ by $hgd$ does not change the contracted prime. Conversely, if $g\mathfrak P$ and $g'\mathfrak P$ contract to the same prime, some $h\in H$ sends the former to the latter, so $g'^{-1}hg\in D$ and $Hg'D=HgD$. This also verifies the stated order of the two sides of the double coset.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 123](../../../paper-123-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
