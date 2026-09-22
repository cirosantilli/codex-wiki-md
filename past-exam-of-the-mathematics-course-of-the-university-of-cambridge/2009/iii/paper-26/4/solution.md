<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**[Galois cohomology](../../../../../galois-cohomology.md) and finite quotients.** Let $k$ be a [number field](../../../../../number-field.md) and $G_k=\operatorname{Gal}(\overline k/k)$ its [absolute Galois group](../../../../../absolute-galois-group.md). For a discrete abelian $G_k$-module $M$, $H^0(k,M)=M^{G_k}$. A continuous 1-cocycle is a map $c:G_k\to M$ with $c_{\sigma\tau}=c_\sigma+\sigma c_\tau$; a coboundary has the form $c_\sigma=\sigma m-m$. Their quotient is $H^1(k,M)$. Short exact sequences of modules give the [long exact sequence in group cohomology](../../../../../long-exact-sequence-in-group-cohomology.md); the connecting map measures the obstruction to lifting a fixed element to a fixed preimage. This interpretation gives a concrete descent map for an [elliptic curve](../../../../../elliptic-curve.md).

For an integer $m\geq2$, multiplication on the geometric points gives the exact sequence

$$
0\longrightarrow E[m]\longrightarrow E(\overline k)\xrightarrow{[m]}E(\overline k)\longrightarrow0.
$$

Here multiplication is a separable isogeny in characteristic zero, with $m^2$ geometric kernel points. For $P\in E(k)$ choose $Q$ with $mQ=P$. Then $c_\sigma=\sigma Q-Q$ lies in $E[m]$, satisfies the cocycle identity, and changing $Q$ changes it by a coboundary. Its class $\delta(P)$ vanishes exactly when $P\in mE(k)$: if $c_\sigma=\sigma T-T$ for $T\in E[m]$, the point $Q-T$ is rational and divides $P$. Thus the [Kummer exact sequence of an elliptic curve](../../../../../kummer-exact-sequence-of-an-elliptic-curve.md) includes

$$
0\longrightarrow E(k)/mE(k)\xrightarrow{\delta}H^1(k,E[m])\longrightarrow H^1(k,E)[m]\longrightarrow0.
$$

The construction also proves that $\delta$ is a homomorphism. The final group can be interpreted as classes of elliptic-curve torsors killed by $m$; imposing soluble completions leads to the [Selmer group of an elliptic curve](../../../../../n-selmer-group.md). For weak Mordell-Weil, the important task is to bound the arithmetic image of $\delta$, not to assume that the entire first cohomology group is finite.

Choose a finite set $S$ containing the bad primes, primes dividing $m$, and archimedean places. At a good finite place $v\notin S$, the class $\delta(P)$ is unramified. Here is the local reason. Over a finite extension of the residue field choose an $m$-division point of the reduction of $P$; multiplication is surjective on the points over its [algebraic closure](../../../../../algebraic-closure.md). Pass to the corresponding unramified extension of $k_v$ and lift this nonsingular point by the [Hensel lemma](../../../../../hensel-s-lemma.md). The discrepancy between $m$ times its lift and $P$ lies in the kernel of reduction. The [formal group of an elliptic curve](../../../../../formal-group-of-an-elliptic-curve.md) describes that kernel, and multiplication by $m$ is bijective there because its leading coefficient is a unit. Correcting the lift therefore gives an actual division point in the unramified closure. Inertia fixes that point, so the Kummer cocycle vanishes on inertia. The same good-reduction argument shows that $E[m]$ itself is unramified outside $S$.

We now prove the required finiteness of unramified cohomology classes. Choose a finite Galois extension $L/k$ over which $E[m]$ and the $m$th roots of unity are all rational, and enlarge $S$ to include its ramified primes. The [inflation-restriction exact sequence](../../../../../inflation-restriction-exact-sequence.md) shows that restriction to $G_L$ has finite kernel: that kernel comes from $H^1(\operatorname{Gal}(L/k),E[m])$, a finite group since both its group and coefficient module are finite. Over $L$, a choice of basis identifies $E[m]$ with $\mu_m^2$. The multiplicative Kummer sequence, together with [Hilbert 90](../../../../../hilbert-s-theorem-90.md), gives

$$
H^1(L,E[m])\cong\bigl(L^\times/L^{\times m}\bigr)^2.
$$

For clarity, [Hilbert 90](../../../../../hilbert-s-theorem-90.md) says that a multiplicative cocycle for a finite Galois extension is a coboundary. If its values are $c_\sigma$, choose $a$ so that $b=\sum_\sigma c_\sigma\sigma(a)\ne0$. Then $\tau(b)=c_\tau^{-1}b$, so $c_\tau=\tau(b^{-1})/b^{-1}$. Such an $a$ exists because distinct [field automorphisms](../../../../../field-automorphism.md) are linearly independent: a relation with the fewest nonzero terms, evaluated on $at$ and compared with its value on $t$ multiplied by one automorphism's value on $a$, would produce a shorter nonzero relation. Continuity reduces the absolute-Galois version to a finite extension. This proves the cohomological vanishing used in the multiplicative Kummer sequence.

An unramified Kummer class represented by $a\in L^\times$ has $v_w(a)\equiv0\pmod m$ at every finite $w\notin S_L$. Indeed an $m$th root of $a$ fixed by inertia belongs to an unramified local extension, whose value group is still the integers. Define

$$
L(S_L,m)=\{[a]\in L^\times/L^{\times m}:v_w(a)\equiv0\pmod m\text{ for }w\notin S_L\}.
$$

Factoring the fractional ideal away from $S_L$ as an $m$th power gives the exact sequence

$$
0\longrightarrow\mathcal O_{L,S_L}^{\times}/\mathcal O_{L,S_L}^{\times m}
\longrightarrow L(S_L,m)
\longrightarrow\operatorname{Cl}(\mathcal O_{L,S_L})[m]\longrightarrow0.
$$

To check it, send $[a]$ to the ideal class of its $m$th root ideal. Changing $a$ by an $m$th power changes that ideal by a principal ideal. The kernel consists precisely of S-units modulo $m$th powers, and every $m$-torsion ideal class has a representative whose $m$th power is principal, proving surjectivity. The [S-unit group](../../../../../s-unit-group.md) is finitely generated by the [Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md) and the finite collection of allowed prime valuations. The localized [ideal class group](../../../../../ideal-class-group.md) is a quotient of the finite ordinary ideal class group. Both end groups, and hence $L(S_L,m)$, are finite. This is the [finiteness of S-unramified Kummer classes](../../../../../finiteness-of-s-unramified-kummer-classes.md) argument.

The restrictions of the elliptic Kummer image lie in two copies of this finite group, and the restriction kernel is finite. The injection $\delta$ therefore proves

$$
\boxed{E(k)/mE(k)\text{ is finite for every }m\geq2.}
$$

This is the [Weak Mordell-Weil theorem](../../../../../weak-mordell-weil-theorem.md). The unramified restriction is essential: even $H^1(k,\mu_2)=k^\times/k^{\times2}$ is generally infinite. Cohomology turns divisibility into a cocycle; [good reduction](../../../../../good-reduction-of-an-elliptic-curve.md) restricts its ramification; units and ideal classes supply the arithmetic finiteness.

**[Height functions](../../../../../height-function.md) and finite generation.** Write $d=[k:\mathbb Q]$ and use absolute values extending the usual rational ones, with local degrees $n_v=[k_v:\mathbb Q_v]$. The logarithmic height of a projective pair is

$$
h(a:b)=\frac1d\sum_v n_v\log\max(|a|_v,|b|_v).
$$

The [product formula](../../../../../product-formula.md) makes it independent of scaling. For $t\in k$, $h(t)=h(t:1)$ is nonnegative. On a short Weierstrass equation $E:y^2=x^3+Ax+B$, put $h_x(P)=h(x(P))$ and $h_x(O)=0$.

Bounded height gives only finitely many [rational points](../../../../../rational-point.md). To see the scalar finiteness behind the [Northcott theorem](../../../../../northcott-theorem.md), an algebraic number $t$ of degree $e$ has primitive minimal polynomial $a_0\prod_{i=1}^e(T-t_i)$, and the product formula gives $e^{e h(t)}=|a_0|\prod_i\max(1,|t_i|)$. If $e\leq d$ and $h(t)\leq H$, every coefficient has absolute value at most $2^d e^{dH}$. There are only finitely many such integer polynomials and hence finitely many roots. Each x-coordinate lifts to at most two points of $E$, with $O$ handled separately. Thus $\{P\in E(k):h_x(P)\leq H\}$ is finite.

The second ingredient is height expansion under doubling:

$$
|h_x(2P)-4h_x(P)|\leq C_E.
$$

Indeed the duplication formula is the degree-four morphism of the projective x-line represented by the coprime quartic forms

$$
F(X,Z)=X^4-2AX^2Z^2-8BXZ^3+A^2Z^4,
$$



$$
G(X,Z)=4X^3Z+4AXZ^3+4BZ^4.
$$

They are coprime because the [elliptic curve](../../../../../elliptic-curve.md) is nonsingular. At each place their coefficient bounds give $\max(|F|_v,|G|_v)\leq C_v\max(|X|_v,|Z|_v)^4$. Bezout identities expressing powers of each coordinate as combinations of $F,G$ give the reverse inequality up to another local constant. One obtains these identities by the Euclidean algorithm on the two affine charts and clearing denominators. Only finitely many non-Archimedean places have a constant different from one. Taking weighted logarithms and summing proves the uniform bounded error. This is [height growth under a morphism of the projective line](../../../../../height-growth-under-a-morphism-of-the-projective-line.md), applied with degree four.

For a fixed $R=(r,s)\in E(k)$, the addition formula also gives

$$
h_x(P-R)\leq2h_x(P)+C_R.
$$

For $x(P)\ne r$, its x-coordinate is

$$
\frac{rx^2+(A+r^2)x+Ar+2B+2sy}{(x-r)^2}.
$$

The curve equation bounds $|y|_v$ by a local constant times $\max(1,|x|_v)^{3/2}$. Both numerator and denominator are consequently bounded by a local constant times $\max(1,|x|_v)^2$. The projective-height definition gives the claimed inequality; the finitely many exceptional points with $x=r$ are absorbed into the constant. For $R=O$ the estimate is immediate.

By weak Mordell-Weil, choose finitely many representatives $R_1,\ldots,R_t$ for $E(k)/2E(k)$. Every $P$ can be written $P=2Q+R_i$. Combining the last two inequalities gives

$$
h_x(Q)\leq\tfrac14h_x(P-R_i)+\tfrac14C_E
\leq\tfrac12h_x(P)+C_0,
$$

with one constant $C_0\geq0$ for all the representatives. This is [naive height contraction in elliptic halving descent](../../../../../naive-height-contraction-in-elliptic-halving-descent.md). If $h_x(P)>2C_0+1$, the new point $Q$ has height at least one half less than that of $P$. Repetition must therefore reach the finite set of points of height at most $2C_0+1$. Reversing the identities $P_j=2P_{j+1}+R_{i_j}$ shows that every point is generated by this finite terminal set together with the finite list of representatives. Thus

$$
\boxed{E(k)\text{ is a finitely generated abelian group}.}
$$

The structure theorem then gives $E(k)\cong E(k)_{\mathrm{tors}}\times\mathbb Z^r$ with finite [torsion subgroup](../../../../../torsion-subgroup.md): this is the [Mordell-Weil theorem](../../../../../mordell-weil-group.md). Finiteness modulo two alone does not imply finite generation; the contracting height argument is what bridges that gap.

The bounded duplication error also constructs the [canonical height of an elliptic curve](../../../../../canonical-height-of-an-elliptic-curve.md):

$$
\widehat h(P)=\frac12\lim_{j\to\infty}4^{-j}h_x(2^jP).
$$

The successive differences are bounded by a summable geometric sequence, so the limit exists, $\widehat h(P)=\tfrac12h_x(P)+O_E(1)$, and $\widehat h(2P)=4\widehat h(P)$. It is nonnegative. Torsion points have canonical height zero because their multiples form a finite set. Conversely, if the canonical height is zero, all $2^jP$ have bounded naive height; Northcott finiteness makes two of them equal and hence makes $P$ torsion. The canonical height removes the bounded error from the arithmetic growth law and identifies exactly the torsion directions, while the elementary naive-height descent already proves finite generation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
