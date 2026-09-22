<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [orientation of a vector bundle](../../../../../orientation-of-a-vector-bundle.md) of real rank $d$ over $R$ is a coherent choice of generator of $H^d(E_b,E_b\setminus\{0\};R)$ in every fibre. For a complex bundle of rank $m$, a complex basis gives the real basis $(v_1,iv_1,\ldots,v_m,iv_m)$. A complex change of basis has positive real determinant $|\det_{\mathbb C}A|^2$, so these local choices agree and give the [canonical orientation of a complex vector bundle](../../../../../canonical-orientation-of-a-complex-vector-bundle.md) over $\mathbb Z$, hence over every commutative ring $R$.

Let $D(E)$ and $S(E)$ be the disk and sphere bundles of an $R$-oriented rank-$d$ bundle over compact $B$. A [Thom class](../../../../../thom-class.md) $u_E\in H^d(D(E),S(E);R)$ restricts to the chosen generator on every fibre. The [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) states that

$$
H^q(B;R)\xrightarrow{\sim}H^{q+d}(D(E),S(E);R),
\qquad a\longmapsto\pi^*a\smile u_E.
$$

The [Euler class of a vector bundle](../../../../../euler-class-of-a-vector-bundle.md) is $e(E)=s^*u_E\in H^d(B;R)$ for the zero section $s$. Substituting the Thom isomorphism into the long exact sequence of the pair $(D(E),S(E))$ gives the [Gysin sequence of a sphere bundle](../../../../../gysin-sequence-of-a-sphere-bundle.md)

$$
\cdots\to H^{q-d}(B;R)\xrightarrow{\smile e(E)}H^q(B;R)\to H^q(S(E);R)\to H^{q-d+1}(B;R)\to\cdots.
$$

Apply this to the [Hopf fibration](../../../../../hopf-fibration.md) and induct on $n$. If $x=c_1(\mathcal O(1))$ has degree two, the result is the [cohomology ring of complex projective space](../../../../../cohomology-ring-of-complex-projective-space.md)

$$
H^*(\mathbb{CP}^n;\mathbb Z)\cong\mathbb Z[x]/(x^{n+1}).
$$

The [Künneth theorem](../../../../../kunneth-theorem.md) over a principal ideal domain gives a natural short exact sequence with tensor-product and Tor terms; the sequence splits, though not naturally. Here all groups are free, so the Tor term vanishes and

$$
H^*(\mathbb{CP}^n\times\mathbb{CP}^n;\mathbb Z)
\cong\mathbb Z[x,y]/(x^{n+1},y^{n+1}).
$$

If a graded-ring automorphism sends $x$ to $ax+by$, then $(ax+by)^{n+1}=0$. The coefficients of the nonzero mixed monomials force $ab=0$; the same applies to the image of $y$. Invertibility then forces a signed permutation matrix on the basis $x,y$. Conversely, complex conjugation on either factor changes the sign of its degree-two generator, and swapping the factors exchanges $x$ and $y$. Thus the realizable group is

$$
\boxed{(\mathbb Z/2)^2\rtimes S_2,}
$$

the group of all signed $2$ by $2$ permutation matrices, as described by the [cohomology automorphisms of a product of two complex projective spaces](../../../../../cohomology-automorphisms-of-a-product-of-two-complex-projective-spaces.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
