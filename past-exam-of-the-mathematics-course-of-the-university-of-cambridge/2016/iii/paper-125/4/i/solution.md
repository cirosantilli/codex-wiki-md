<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Heights measure arithmetic size, and their finiteness and growth properties turn finite divisibility information into finite generation. For an [elliptic curve](../../../../../../elliptic-curve.md) $E$ over a [number field](../../../../../../number-field.md) $K$, the resulting [Mordell-Weil theorem](../../../../../../mordell-weil-group.md) is

$$
\boxed{E(K)\cong\mathbb Z^r\oplus E(K)_{\mathrm{tors}},\qquad r<\infty,\quad\#E(K)_{\mathrm{tors}}<\infty.}
$$

The distinction between this statement and the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md), which only asserts that $E(K)/mE(K)$ is finite, is exactly where heights enter.

For a rational point of the projective line, choose coprime integers $a,b$ and define the logarithmic [projective height](../../../../../../projective-height.md)

$$
h([a:b])=\log\max(|a|,|b|).
$$

For a fixed number field, its absolute logarithmic version is

$$
h([a:b])=\frac1{[K:\mathbb Q]}\sum_v n_v\log\max(|a|_v,|b|_v),\qquad n_v=[K_v:\mathbb Q_v],
$$

with the usual normalized absolute values. The [product formula](../../../../../../product-formula.md) makes this independent of scaling $(a,b)$, and the local degree formula makes it independent of enlarging the number field. Heights are nonnegative and are useful precisely because they control numerator and denominator together, unlike an ordinary real absolute value.

The [Northcott theorem](../../../../../../northcott-theorem.md) states that algebraic points of bounded degree and bounded height form a finite set. Over $\mathbb Q$ this is immediate from the coprime numerator-denominator description. In general, bounded degree and height bound the coefficients of the primitive minimal polynomial: their elementary symmetric functions are bounded by its Mahler measure, which is the appropriate power of the multiplicative height. There are only finitely many such integer polynomials.

On a [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md), define the naive logarithmic height $h_x(P)=h(x(P))$ and $h_x(O)=0$. Since an $x$-coordinate has at most two points above it, [Northcott theorem](../../../../../../northcott-theorem.md) implies that only finitely many points of $E(K)$ have bounded $h_x$.

Duplication descends to a rational map of the projective $x$-line of degree $4$. More generally, if a morphism $\phi:\mathbb P^1\to\mathbb P^1$ has degree $d$, then

$$
h(\phi(z))=d\,h(z)+O(1),
$$

uniformly in $z$. Write $\phi$ as two homogeneous degree-$d$ polynomials without common zeros. Bounding their coefficients gives the upper estimate at each place. A nonzero [resultant](../../../../../../resultant.md), or homogeneous Bezout identities, prevents simultaneous cancellation and gives the lower estimate; only finitely many places contribute a nonzero constant. Applied to duplication, this gives the [height growth under a morphism of the projective line](../../../../../../height-growth-under-a-morphism-of-the-projective-line.md) estimate

$$
|h_x(2P)-4h_x(P)|\leq C_E.
$$

Define the [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md) by

$$
\boxed{\widehat h(P)=\frac12\lim_{n\to\infty}4^{-n}h_x(2^nP).}
$$

The factor $1/2$ is a convention making it the height for the degree-one symmetric divisor $O$. If $a_n=4^{-n}h_x(2^nP)$, then $|a_{n+1}-a_n|\leq C_E4^{-(n+1)}$, so the limit exists by a geometric-series estimate. Summing that estimate also proves

$$
\left|\widehat h(P)-\tfrac12h_x(P)\right|\leq C_E/6.
$$

Thus bounded canonical height still gives only finitely many $K$-points, and $\widehat h(2P)=4\widehat h(P)$ exactly.

The addition formula on the quotient by negation gives the uniform approximate parallelogram identity

$$
h_x(P+Q)+h_x(P-Q)=2h_x(P)+2h_x(Q)+O(1).
$$

This [height parallelogram identity](../../../../../../height-parallelogram-identity.md) follows as follows. One way to obtain it is to express the unordered pair of their $x$-coordinates as a morphism $\mathbb P^1\times\mathbb P^1\to\operatorname{Sym}^2\mathbb P^1$ of bidegree $(2,2)$; the height of that unordered pair is the sum of the two heights, up to a bounded constant. It is also the height identity for the symmetric divisor $O$. Apply this identity to $2^nP,2^nQ$, divide by $2\cdot4^n$, and take limits. The errors disappear, giving

$$
\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).
$$

Together with evenness and $\widehat h(O)=0$, the recurrence implies $\widehat h(mP)=m^2\widehat h(P)$ for every integer $m$. The associated [canonical height pairing](../../../../../../canonical-height-pairing.md)

$$
\langle P,Q\rangle=\tfrac12\bigl(\widehat h(P+Q)-\widehat h(P)-\widehat h(Q)\bigr)
$$

is bilinear. Nonnegativity of the height implies its [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), by applying it to integer combinations and then rational approximations. In particular,

$$
\widehat h(P-Q)\leq2\widehat h(P)+2\widehat h(Q).
$$

The height vanishes precisely at torsion points: torsion gives a finite set of multiples, whereas if $\widehat h(P)=0$, every multiple of $P$ has bounded naive height and therefore the set of multiples is finite by [Northcott theorem](../../../../../../northcott-theorem.md).

Now apply the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md) with $m=2$, proved cohomologically in the other essay. Choose a finite set $R$ of representatives for $E(K)/2E(K)$, and put $H=\max_{R_i\in R}\widehat h(R_i)$. Write an arbitrary point as $P=2Q+R_i$. Then

$$
\widehat h(Q)=\tfrac14\widehat h(P-R_i)\leq\tfrac12\widehat h(P)+\tfrac12H.
$$

If $\widehat h(P)>H+1$, this decreases the height by more than $1/2$. Repeat until the current point has height at most $H+1$. There are only finitely many such points. Unwinding the equations $P=2Q+R_i$ shows that $E(K)$ is generated by this finite bounded-height set together with $R$. This is the [height descent lemma](../../../../../../height-descent-lemma.md), and proves the [Mordell-Weil theorem](../../../../../../mordell-weil-group.md).

Once finite generation is established, the structure theorem for finitely generated abelian groups gives the displayed decomposition. The [canonical height pairing](../../../../../../canonical-height-pairing.md) is positive definite on the real vector space of the free part: a null direction would, by approximation with integer combinations of generators, give infinitely many lattice points of bounded height, contradicting [Northcott theorem](../../../../../../northcott-theorem.md). Its determinant is the [regulator of an elliptic curve](../../../../../../regulator-of-an-elliptic-curve.md), and its geometry gives practical tools for searching for generators and comparing independence. Thus heights supply both the finiteness mechanism in the proof and the quadratic size function used in arithmetic computations.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
