<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [height function](../../../../../../height-function.md) measures arithmetic size, which is what makes an otherwise infinite descent terminate. For a [number field](../../../../../../number-field.md) $K$, normalize absolute values to extend the standard real and $p$-adic ones, and write $n_v=[K_v:\mathbb Q_v]$. The logarithmic [projective height](../../../../../../projective-height.md) is

$$
h([a_0:\cdots:a_s])=\frac1{[K:\mathbb Q]}\sum_v n_v\log\max_j|a_j|_v.
$$

The [product formula](../../../../../../product-formula.md) makes it independent of the chosen homogeneous coordinates, and the local-degree normalization makes it independent of the [number field](../../../../../../number-field.md) containing them. Over $\mathbb Q$, $h([a:b])=\log\max(|a|,|b|)$ for [coprime](../../../../../../coprime-integers.md) integer coordinates. Set $h_x(P)=h(x(P))$ on an [elliptic curve](../../../../../../elliptic-curve.md), with $h_x(O)=0$.

Two features are essential. First, the [Northcott theorem](../../../../../../northcott-theorem.md) says that points of bounded [projective height](../../../../../../projective-height.md) and bounded field degree form a finite set. For points on a fixed [elliptic curve](../../../../../../elliptic-curve.md) over $K$, each $x$-coordinate has at most two preimages, so bounded $h_x$ gives finitely many points. Second, a degree-$d$ morphism of the [projective line](../../../../../../projective-line.md) satisfies $h(f(z))=dh(z)+O(1)$, uniformly in $z$. The upper bound comes from evaluating its homogeneous [polynomials](../../../../../../polynomial-split.md); for the lower bound, their lack of a common zero gives a resultant identity bounding the input coordinates by the output coordinates at each place. Summing the local bounds gives the asserted uniform constant.

The duplication map on the $x$-line has degree four. Nonsingularity ensures that its numerator and denominator have no common projective zero. Therefore

$$
h_x(2P)=4h_x(P)+O(1).
$$

Telescoping defines the [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md)

$$
\widehat h(P)=\frac12\lim_{j\to\infty}4^{-j}h_x(2^jP),\qquad
\widehat h(P)=\tfrac12h_x(P)+O(1).
$$

The error in successive terms is bounded by a geometric series, proving convergence and the uniform bounded difference. It also gives $\widehat h(2P)=4\widehat h(P)$ and nonnegativity. The usual addition formula gives the approximate [height parallelogram identity](../../../../../../height-parallelogram-identity.md) for $h_x$; equivalently, the unordered pair of sum and difference on the $x$-line has bidegree $(2,2)$. Applying that identity to $2^jP,2^jQ$ and passing to the limit gives

$$
\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).
$$

In particular $\widehat h(nP)=n^2\widehat h(P)$. Its polarization is the [canonical height pairing](../../../../../../canonical-height-pairing.md), a positive semidefinite bilinear form even before finite generation has been proved. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) for this pairing gives

$$
\widehat h(P-Q)\leq2\widehat h(P)+2\widehat h(Q).
$$

Also $\widehat h(P)=0$ precisely for [torsion points of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md): one direction follows from periodic multiples, and in the other direction all multiples have bounded $h_x$, so the [Northcott theorem](../../../../../../northcott-theorem.md) makes two multiples equal. Bounded [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md) likewise gives a finite set of $K$-[rational points](../../../../../../rational-point.md).

Now the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md) gives finitely many representatives $R_1,\ldots,R_s$ for $E(K)/2E(K)$. Put $H=\max_i\widehat h(R_i)$. Write any point as $P=2Q+R_i$. Then

$$
\widehat h(Q)=\tfrac14\widehat h(P-R_i)
\leq\tfrac12\widehat h(P)+\tfrac12H.
$$

Repeatedly applying this [height descent lemma](../../../../../../height-descent-lemma.md) eventually reaches height at most $H+1$: after $j$ steps the height is at most $H+2^{-j}(\widehat h(P)-H)$. The set of points with height at most $H+1$ is finite. Reading the relations $P=2Q+R_i$ backwards shows that this finite set together with the $R_i$ generates $E(K)$. Consequently

$$
\boxed{E(K)\cong E(K)_{\mathrm{tors}}\oplus\mathbb Z^r,\qquad r<\infty.}
$$

**Heights turn weak Mordell-Weil finiteness into the Mordell-Weil theorem.** The [canonical height pairing](../../../../../../canonical-height-pairing.md) subsequently equips the free part with a positive definite [quadratic form](../../../../../../quadratic-form.md), useful for bounding searches and measuring independent generators; this interpretation is a consequence of the proof, not an assumption used in the descent.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
