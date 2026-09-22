<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Arithmetic heights](../../../../../../height-function.md) measure arithmetic complexity. For a reduced [rational number](../../../../../../rational-number.md) $x=a/b$, its [multiplicative height](../../../../../../absolute-multiplicative-weil-height.md) is $H(x)=\max(|a|,|b|)$ and its [logarithmic height](../../../../../../absolute-logarithmic-weil-height.md) is $h(x)=\log H(x)$. Over a [number field](../../../../../../number-field.md) $K$, use the absolute [projective height](../../../../../../projective-height.md)

$$
h([x_0:\cdots:x_d])=\frac1{[K:\mathbb Q]}\sum_v[K_v:\mathbb Q_v]\log\max_i|x_i|_v.
$$

Normalize the [absolute values on a field](../../../../../../absolute-value-algebra.md) by the [product formula](../../../../../../product-formula.md). That formula makes [arithmetic height](../../../../../../height-function.md) independent of the chosen homogeneous representative, and the normalization makes it independent of enlarging $K$. The [Northcott theorem](../../../../../../northcott-theorem.md) says that algebraic points of bounded degree and bounded [arithmetic height](../../../../../../height-function.md) form a [finite set](../../../../../../finite-set.md). For [rational numbers](../../../../../../rational-number.md) this follows immediately by bounding the numerator and denominator. In a fixed [number field](../../../../../../number-field.md), the same finiteness follows by bounding the coefficients of the [minimal polynomial](../../../../../../minimal-polynomial.md) using its conjugates and the [arithmetic height](../../../../../../height-function.md).

For an [elliptic curve](../../../../../../elliptic-curve.md) put $h_x(P)=h([x(P):1])$ and $h_x(O)=0$. The two points above a given $x$ show that bounded $h_x$ gives finitely many $K$-rational points. More importantly, multiplication expands this [arithmetic height](../../../../../../height-function.md). To see the mechanism, choose a short [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) $y^2=x^3+Ax+B$ over $K$. Doubling gives

$$
x(2P)=\frac{x(P)^4-2Ax(P)^2-8Bx(P)+A^2}{4(x(P)^3+Ax(P)+B)}.
$$

After homogenization the numerator and denominator are quartics with no common zero. At infinity the numerator is nonzero; at a root $t$ of the cubic the numerator becomes $(3t^2+A)^2$, nonzero by nonsingularity. For a degree-$d$ morphism of the [projective line](../../../../../../projective-line.md), fixed homogeneous coefficients give the upper [arithmetic height](../../../../../../height-function.md) bound $h(f(x))\leq d h(x)+C$. A nonzero resultant supplies the reverse bound: at each place it bounds the common cancellation of the two homogeneous values, with a nontrivial constant needed at only finitely many places. Applying these bounds to duplication gives a constant $C$ independent of $P$ with

$$
|h_x(2P)-4h_x(P)|\leq C.
$$

This includes points mapping to $O$, by the projective formulation.

The [canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) removes the bounded errors. With the conventional factor one half, define

$$
\widehat h(P)=\frac12\lim_{n\to\infty}4^{-n}h_x(2^nP).
$$

The successive terms before multiplying by one half differ by at most $C4^{-n-1}$. The limit exists, and summing this geometric bound gives

$$
|\widehat h(P)-\tfrac12h_x(P)|\leq C/6,\qquad \widehat h(2P)=4\widehat h(P),\qquad\widehat h(P)\geq0.
$$

Hence bounded [canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) still gives finitely many points over the fixed [number field](../../../../../../number-field.md).

To obtain the pairing, the quadratic nature comes from a uniform [arithmetic height](../../../../../../height-function.md) parallelogram estimate, not just from doubling. If $x=x(P)$ and $z=x(Q)$, the unordered coordinates $x(P+Q),x(P-Q)$ are the roots of the binary quadratic with coefficients

$$
C_2=(x-z)^2,\quad C_1=2(xz+A)(x+z)+4B,\quad C_0=(xz-A)^2-4B(x+z).
$$

These formulas follow by adding and multiplying the two chord expressions with slopes $(y(P)-y(Q))/(x-z)$ and $(y(P)+y(Q))/(x-z)$. Their homogenizations have bidegree $(2,2)$ and no simultaneous zero. Off the diagonal $C_2\ne0$; on the finite diagonal $x=z=t$, $C_1=4f(t)$ and $C_0=f'(t)^2-8tf(t)$ for $f(t)=t^3+At+B$, so simultaneous vanishing would contradict nonsingularity. At the double point at infinity the homogeneous $C_0$ is nonzero. Local coefficient norms, or the corresponding resultant bounds, therefore give

$$
h([C_0:C_1:C_2])=2h_x(P)+2h_x(Q)+O(1).
$$

The [arithmetic height](../../../../../../height-function.md) of a binary quadratic's coefficient vector differs by $O(1)$ from the sum of the heights of its two roots. At finite places this follows from multiplicativity of the maximum coefficient norm of products; at infinite places the fixed-degree norms are comparable. Thus

$$
h_x(P+Q)+h_x(P-Q)=2h_x(P)+2h_x(Q)+O(1).
$$

Apply this to $2^nP,2^nQ$, divide by $2\cdot4^n$ and take limits. The errors vanish and give the exact [height parallelogram identity](../../../../../../height-parallelogram-identity.md). Polarization consequently makes

$$
\langle P,Q\rangle=\frac12(\widehat h(P+Q)-\widehat h(P)-\widehat h(Q))
$$

a symmetric [bilinear](../../../../../../bilinear-map.md) pairing. Nonnegativity of $\widehat h(aP+bQ)$ for [integers](../../../../../../integer.md) $a,b$, and density of rational ratios, give the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). In particular $\widehat h(P-Q)\leq2\widehat h(P)+2\widehat h(Q)$. Also $\widehat h(mP)=m^2\widehat h(P)$ for [integers](../../../../../../integer.md) $m$. [Torsion points of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md) have [canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) zero because their doubling orbit is finite; conversely, if a point has [canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) zero, all its [integer](../../../../../../integer.md) multiples have bounded [naive height](../../../../../../naive-height-on-the-projective-line.md), and finiteness forces two multiples to coincide. Thus [canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) vanishes exactly on torsion.

There is an arithmetic finiteness input before [height descent](../../../../../../height-descent-lemma.md): $E(K)/2E(K)$ is finite, the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md). Here is its mechanism. The multiplication [exact sequence](../../../../../../exact-sequence.md) gives an injective Kummer map $E(K)/2E(K)\to H^1(K,E[2])$: choose a half-point $Q$ and use the cocycle $\sigma\mapsto\sigma Q-Q$; changing $Q$ changes a coboundary, and a trivial class means a half-point can be chosen over $K$. Let $L=K(E[2])$, a [Finite Galois extension](../../../../../../finite-galois-extension.md). Over $L$ the [torsion module](../../../../../../torsion-module.md) is $(\mathbb Z/2\mathbb Z)^2$, so [Kummer theory](../../../../../../kummer-theory.md) identifies its first [Galois cohomology](../../../../../../galois-cohomology.md) with two copies of $L^\times/L^{\times2}$.

Only classes unramified outside a fixed [finite set](../../../../../../finite-set.md) $S$ occur. Include the [primes](../../../../../../prime-number.md) over $2$, bad-reduction [primes](../../../../../../prime-number.md) and the ramified [primes](../../../../../../prime-number.md) of $L/K$. At a good [prime](../../../../../../prime-number.md) away from $2$, multiplication by two on the proper smooth elliptic model is [finite étale morphism](../../../../../../finite-etale-morphism.md), so the torsor of halves of a point is unramified. In square-class language, [valuations](../../../../../../valuation.md) outside $S$ are even. Such classes form a [finite group](../../../../../../finite-group.md): write the [principal ideal](../../../../../../principal-ideal.md) of a representative as a square times an ideal supported on $S$. The ideal class gives an element of the finite two-torsion of the localized [ideal class group](../../../../../../ideal-class-group.md); after fixing that class, ambiguity is an $S$-unit modulo squares. The $S$-unit theorem makes the latter finite. The [group kernel](../../../../../../kernel-of-a-group-homomorphism.md) of restriction from $K$ to $L$ is contained in $H^1(\operatorname{Gal}(L/K),E[2])$, which is finite because both the group and module are finite. This proves the weak theorem, without assuming finite generation of $E(K)$.

Finally choose representatives $R_1,\ldots,R_s$ of $E(K)/2E(K)$ and put $M=\max_i\widehat h(R_i)$. Every $P$ has the form $2Q+R_i$, and

$$
\widehat h(Q)=\frac14\widehat h(P-R_i)\leq\frac12\widehat h(P)+\frac12M.
$$

If $\widehat h(P)>M+1$, this reduces [canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) by more than one half. Iterate until a point of [canonical height](../../../../../../canonical-height-of-an-elliptic-curve.md) at most $M+1$ is reached. There are only finitely many such points, by Northcott and the bounded difference of heights. Reconstructing $P=2Q+R_i$ at every stage proves that these finitely many small points and the finitely many representatives generate $E(K)$. Therefore

$$
\boxed{E(K)\cong E(K)_{\mathrm{tors}}\oplus\mathbb Z^r\quad\text{for some finite }r.}
$$

The canonical pairing is positive definite on the free part. It turns rank computations into an arithmetic lattice problem, supplies independence tests for proposed generators, and bounds searches once a [arithmetic height](../../../../../../height-function.md) bound is available. Weak finite-quotient finiteness alone would not prove this result: the [arithmetic height](../../../../../../height-function.md) contraction is the step that converts it into finite generation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
