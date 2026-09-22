<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K$ be a [number field](../../../../../../number-field.md) and $E/K$ an [elliptic curve](../../../../../../elliptic-curve.md). Heights measure the arithmetic size of points, and turn the finite quotient supplied by the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md) into finite generation. For a [projective point](../../../../../../projective-point.md) $[X:Z]\in\mathbb P^1(K)$ define the [Absolute logarithmic Weil height](../../../../../../absolute-logarithmic-weil-height.md)

$$
h([X:Z])=\frac1{[K:\mathbb Q]}\sum_v n_v\log\max(|X|_v,|Z|_v),
$$

using the usual normalized absolute values and local degrees $n_v=[K_v:\mathbb Q_v]$. The [product formula](../../../../../../product-formula.md) makes this independent of scaling and of enlarging $K$. For a [Short Weierstrass form](../../../../../../short-weierstrass-form.md) put $h_x(P)=h([x(P):1])$ and $h_x(O)=h([1:0])=0$. Over $\mathbb Q$, if $x=A/B$ in lowest terms, $h(x)=\log\max(|A|,|B|)$.

The finiteness property is [Northcott theorem](../../../../../../northcott-theorem.md): for bounded height and bounded degree over $\mathbb Q$ there are only finitely many algebraic numbers. One sees the mechanism from the [height-Mahler measure formula](../../../../../../height-mahler-measure-formula.md). If $\alpha$ has degree $d\le D$ and height at most $H$, its primitive integral [minimal polynomial](../../../../../../minimal-polynomial.md) has [Mahler measure](../../../../../../mahler-measure.md) $e^{dh(\alpha)}\le e^{DH}$. Expanding its product of linear factors bounds every coefficient by $2^De^{DH}$. Only finitely many integral [polynomials](../../../../../../polynomial-split.md) satisfy this bound, and each has finitely many roots. Thus a height bound gives only finitely many $x$-coordinates in the fixed [number field](../../../../../../number-field.md) $K$, and each gives at most two points of $E$, besides $O$.

To understand multiplication, the doubling formula gives

$$
x(2P)=\frac{x^4-2ax^2-8bx+a^2}{4(x^3+ax+b)}.
$$

Its homogeneous numerator and denominator have degree four. They have no common projective zero: at infinity the numerator is nonzero, and at a root of $f(t)=t^3+at+b$ the numerator equals $f'(t)^2$, since it is $f'(t)^2-8tf(t)$. Nonsingularity excludes a common root of $f,f'$. The coordinate doubling map is therefore a degree-four morphism of the [projective line](../../../../../../projective-line.md).

The general [height growth under a morphism of the projective line](../../../../../../height-growth-under-a-morphism-of-the-projective-line.md) is $h(\Phi(t))=d h(t)+O(1)$ for a fixed degree-$d$ morphism. Here is why the error is bounded independently of $t$. At a place $v$, normalize its homogeneous coordinates to have maximum norm $1$. The fixed homogeneous forms have uniformly bounded norm. They also have a positive lower bound: the normalized coordinate space is compact over $K_v$, and their common zero [set](../../../../../../set-split.md) is empty. Outside finitely many places their coefficients are integral and their reduction has no common zero, making both bounds $1$. Homogeneity and summation over places then give the asserted height estimate. Consequently there is a fixed $C$ with

$$
|h_x(2P)-4h_x(P)|\le C\qquad(P\in E(K)).
$$

Define the [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md) by the conventional normalization

$$
\widehat h(P)=\frac12\lim_{n\to\infty}4^{-n}h_x(2^nP).
$$

The successive approximants differ by at most $C/(2\cdot4^{n+1})$, so the limit exists and

$$
\left|\widehat h(P)-\tfrac12h_x(P)\right|\le\frac C6,
\qquad \widehat h(2P)=4\widehat h(P),\qquad\widehat h(P)\ge0.
$$

Thus [canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) retains Northcott finiteness, while replacing the bounded-error doubling rule by an exact one.

We also need the [height parallelogram identity](../../../../../../height-parallelogram-identity.md). It follows from the [symmetric-square proof of the naive height parallelogram estimate](../../../../../../symmetric-square-proof-of-the-naive-height-parallelogram-estimate.md), which we give explicitly using the supplied addition formulae. For $x_i=X_i/Z_i$, the unordered pair $x(P+Q),x(P-Q)$ is represented by the binary quadratic $CT^2-BTS+AS^2$, where

$$
\begin{aligned}
A&=X_1^2X_2^2-2aX_1X_2Z_1Z_2-4b(X_1Z_1Z_2^2+X_2Z_2Z_1^2)+a^2Z_1^2Z_2^2,\\
B&=2(X_1X_2+aZ_1Z_2)(X_1Z_2+X_2Z_1)+4bZ_1^2Z_2^2,\\
C&=(X_1Z_2-X_2Z_1)^2.
\end{aligned}
$$

These forms define the [biquadratic morphism for elliptic sums and differences](../../../../../../biquadratic-morphism-for-elliptic-sums-and-differences.md). They have no common zero. If $C=0$, the two projective coordinates agree. On the finite diagonal $x_1=x_2=t$, $B=4f(t)$ and $A=f'(t)^2-8tf(t)$, so simultaneous vanishing would violate nonsingularity. At $(\infty,\infty)$ the homogeneous $A$ is nonzero. This also handles $P=\pm Q$ and sums or differences equal to $O$, for which the affine fractions alone would be inappropriate.

The same local norm argument as above, now using bidegree $(2,2)$, gives

$$
h([A:B:C])=2h_x(P)+2h_x(Q)+O(1).
$$

On the other hand the binary quadratic is the product of two linear factors for $x(P+Q)$ and $x(P-Q)$. At nonarchimedean places coefficient maximum norms multiply exactly: scale each factor to norm $1$ and reduce; the product of the two nonzero residue [polynomials](../../../../../../polynomial-split.md) remains nonzero. This is [multiplicativity of the nonarchimedean polynomial norm](../../../../../../multiplicativity-of-the-nonarchimedean-polynomial-norm.md). At archimedean places the norms are comparable up to fixed constants, by the coefficient triangle inequality and [compactness](../../../../../../compact-space.md) of normalized linear factors. Therefore

$$
h([A:B:C])=h_x(P+Q)+h_x(P-Q)+O(1).
$$

Combining the estimates proves the naive-height parallelogram relation with a uniform error. Apply it to $2^nP,2^nQ$, divide by $2\cdot4^n$, and pass to the limit to obtain

$$
\boxed{\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).}
$$

As in the polarization argument of (a), this makes $\widehat h$ quadratic, with the [canonical height pairing](../../../../../../canonical-height-pairing.md)

$$
\langle P,Q\rangle=\frac{\widehat h(P+Q)-\widehat h(P)-\widehat h(Q)}2,
\qquad \widehat h(nP)=n^2\widehat h(P).
$$

A torsion point has [canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) zero because its multiples have bounded [naive height](../../../../../../naive-height-on-the-projective-line.md). Conversely, if $\widehat h(P)=0$, then all $2^nP$ have bounded [naive height](../../../../../../naive-height-on-the-projective-line.md). Northcott finiteness makes two equal, giving $(2^j-2^i)P=O$ for some $j>i$. Thus **[canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) vanishes exactly on torsion**. In particular the [torsion subgroup](../../../../../../torsion-subgroup.md) is finite, since the comparison with [naive height](../../../../../../naive-height-on-the-projective-line.md) bounds the heights of all its points.

We can now prove the [Mordell-Weil theorem](../../../../../../mordell-weil-group.md). The [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md), as explained in Question 2(ii), makes $E(K)/2E(K)$ finite. Choose representatives $R_1,\ldots,R_s$ and put $M=\max_i\widehat h(R_i)$. Every $P$ can be written $P=2Q+R_i$. The parallelogram identity and nonnegativity give

$$
\widehat h(Q)=\tfrac14\widehat h(P-R_i)\le\tfrac12\widehat h(P)+\tfrac12M.
$$

Iterating this [height descent](../../../../../../height-descent-lemma.md) makes the height at step $n$ at most $M+2^{-n}\max(\widehat h(P)-M,0)$, so after finitely many steps it is at most $M+1$. There are only finitely many points of that height by Northcott and the naive-height comparison. Reversing $P=2Q+R_i$ shows that every point is an [integer](../../../../../../integer.md) combination of the finitely many representatives and this finite bounded-height [set](../../../../../../set-split.md). Therefore

$$
\boxed{E(K)\text{ is finitely generated},\qquad E(K)\cong\mathbb Z^r\oplus E(K)_{\mathrm{tors}}.}
$$

On the resulting free part the [canonical height pairing](../../../../../../canonical-height-pairing.md) is positive definite. Its nonnegativity extends from rational vectors to real vectors by density. If a nonzero real vector $v$ were in its kernel, in a basis of the free part round $nv$ to [integer](../../../../../../integer.md) vectors $z_n$. Their rounding errors are uniformly bounded, and $\widehat h(z_n)=\widehat h(z_n-nv)$ would be uniformly bounded. The vectors $z_n$ are unbounded and therefore include infinitely many distinct vectors, contradicting Northcott finiteness. Thus there is no real null vector. Heights consequently support quantitative point searches, tests of independence, and the [regulator of an elliptic curve](../../../../../../regulator-of-an-elliptic-curve.md), in addition to providing the descent that proves finite generation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
