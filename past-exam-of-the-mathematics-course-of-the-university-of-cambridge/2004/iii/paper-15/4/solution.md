<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Fix an [elliptic curve](../../../../../elliptic-curve.md) $E/K$ with origin $O$ and a [Weierstrass equation of an elliptic curve](../../../../../weierstrass-equation-of-an-elliptic-curve.md). Define the naive logarithmic $x$-height by $h_x(P)=h([x(P):1])$ for $P\ne O$ and $h_x(O)=0$. The $x$-map has degree two and pulls the projective hyperplane bundle back to $\mathcal O_E(2[O])$. Thus

$$
h_E(P)=\tfrac12h_x(P)
$$

is a [Weil height machine](../../../../../weil-height-machine.md) representative for the symmetric ample line bundle $L=\mathcal O_E([O])$. This factor of one half fixes the convention for the [normalized height on an elliptic curve](../../../../../canonical-height-of-an-elliptic-curve.md) used below.

The [Theorem of the Cube](../../../../../theorem-of-the-cube.md) gives the quadratic geometric identities. Pull its alternating line-bundle identity back along $(P,Q)\mapsto(P,Q,-Q)$ and use $[-1]^*L\cong L$. For the addition and subtraction maps $m,d:E^2\to E$, this gives

$$
m^*L\otimes d^*L\cong p_1^*L^{\otimes2}\otimes p_2^*L^{\otimes2}.
$$

On heights, therefore,

$$
h_E(P+Q)+h_E(P-Q)=2h_E(P)+2h_E(Q)+O(1),
$$

uniformly on $E(K)^2$. In particular, restriction to the diagonal gives $[2]^*L\cong L^{\otimes4}$ and a uniform constant $C$ with $|h_E(2P)-4h_E(P)|\leq C$. The general multiplication formula is $[n]^*L\cong L^{\otimes n^2}$: the cube identity applied to $[n],[1],[-1]$ gives a second-difference recurrence, whose initial classes are $[0]^*L=0$ and $[1]^*L=L$ in the Picard group.

Define the [canonical height of an elliptic curve](../../../../../canonical-height-of-an-elliptic-curve.md) by

$$
\boxed{\widehat h(P)=\lim_{n\to\infty}4^{-n}h_E(2^nP)=\frac12\lim_{n\to\infty}4^{-n}h_x(2^nP).}
$$

The existence and bounded comparison are elementary: consecutive terms differ by at most $C4^{-n-1}$, so their telescoping series converges and

$$
|\widehat h(P)-h_E(P)|\leq C/3.
$$

The bound is uniform in $P$, and the limit is nonnegative. Shifting the index gives $\widehat h(2P)=4\widehat h(P)$. This is the unique function within bounded distance of $h_E$ with that doubling rule: the difference of two such functions at $P$ is $4^{-n}$ times their bounded difference at $2^nP$, and hence zero. A change of Weierstrass model changes the naive height only by a bounded function, so the normalized limit is independent of that model.

Apply the approximate parallelogram identity to $2^nP,2^nQ$, divide by $4^n$, and pass to the limit. The bounded error disappears, yielding the exact [height parallelogram identity](../../../../../height-parallelogram-identity.md)

$$
\boxed{\widehat h(P+Q)+\widehat h(P-Q)=2\widehat h(P)+2\widehat h(Q).}
$$

Evenness follows already from $x(-P)=x(P)$. The second-difference recurrence along $nP$, with initial values at $0,P$, consequently gives **$\widehat h(nP)=n^2\widehat h(P)$ for every integer $n$**. The arithmetic cube identity from 2(i), scaled in the same way, also becomes an exact third-difference identity for $\widehat h$.

The [canonical height pairing](../../../../../canonical-height-pairing.md)

$$
\langle P,Q\rangle=\tfrac12\bigl(\widehat h(P+Q)-\widehat h(P)-\widehat h(Q)\bigr)
$$

is symmetric and biadditive: the difference $\langle P+Q,R\rangle-\langle P,R\rangle-\langle Q,R\rangle$ is half the vanishing third difference. Its diagonal is $\widehat h(P)$. Positivity gives the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) for this pairing without first assuming finite generation. Indeed $\widehat h(mP+nQ)\geq0$ for integers $m,n$; dividing by $n^2$ and using density of rational $m/n$ shows that the associated quadratic polynomial is nonnegative on the real line. Its discriminant therefore gives $\langle P,Q\rangle^2\leq\widehat h(P)\widehat h(Q)$.

The [Northcott theorem](../../../../../northcott-theorem.md) and the bounded comparison make $\{P\in E(K):\widehat h(P)\leq B\}$ finite. The map $x:E\to\mathbb P^1$ has finite fibres, so bounded $x$-height indeed controls the number of points, including $O$. This proves the important criterion

$$
\boxed{\widehat h(P)=0\iff P\text{ is torsion}.}
$$

For a torsion point the integer quadratic rule gives zero. Conversely, height zero makes all $2^nP$ belong to one finite bounded-height set; two coincide, forcing $(2^j-2^i)P=O$ for some $j>i$. This argument also proves torsion finiteness over the fixed number field.

The normalized height is functorial for an [isogeny of elliptic curves](../../../../../isogeny-of-elliptic-curves.md) $\phi:E\to E'$:

$$
\widehat h_{E'}(\phi P)=\deg(\phi)\widehat h_E(P).
$$

The pullback of $\mathcal O_{E'}([O'])$ has degree $\deg\phi$ and is symmetric. Its difference from that many copies of $[O]$ is a symmetric degree-zero line bundle, hence a two-torsion Picard class. Its height is bounded, so the ordinary height relation has a bounded error. Commuting the isogeny with $[2^n]$ and taking the normalized limit removes that error. This explains the natural quadratic scaling under multiplication and the usefulness of normalized heights in comparing isogenous curves.

Here is their role in the [Mordell-Weil theorem](../../../../../mordell-weil-group.md). The separate arithmetic input is the [Weak Mordell-Weil theorem](../../../../../weak-mordell-weil-theorem.md), asserting finiteness of $E(K)/2E(K)$. One route uses the [Kummer exact sequence of an elliptic curve](../../../../../kummer-exact-sequence-of-an-elliptic-curve.md) to inject this quotient into $H^1(K,E[2])$. The division torsors are unramified outside finitely many places containing those over $2$ and those of bad reduction. After a finite Galois extension splitting $E[2]$, their classes are pairs of square classes with even valuations outside this finite set. These square classes form a finite group: the obstruction to being represented by an S-unit lies in the finite ideal class group's two-torsion, and the S-unit group is finitely generated, hence finite modulo squares. The inflation-restriction kernel is a cohomology group of a finite group with finite coefficients, also finite. This supplies the finite quotient without using the full theorem in advance.

Choose representatives $R_1,\ldots,R_s$ for that finite quotient and put $H=\max_i\widehat h(R_i)$. Every point has the form $P=2Q+R_i$. Nonnegativity and the exact parallelogram identity give

$$
\widehat h(Q)=\tfrac14\widehat h(P-R_i)\leq\tfrac12\bigl(\widehat h(P)+\widehat h(R_i)\bigr)\leq\frac{\widehat h(P)+H}{2}.
$$

If $\widehat h(P)>H+1$, this decreases the height by more than $1/2$. Repeating must reach the finite set $T=\{P:\widehat h(P)\leq H+1\}$. Unwinding the halving expressions writes the initial point as an integer linear combination of the $R_i$ and a point of $T$. Thus **$E(K)$ is finitely generated**, the [canonical-height proof of Mordell-Weil finite generation](../../../../../canonical-height-proof-of-mordell-weil-finite-generation.md). The normalized height supplies the descent and Northcott supplies its finite endpoint; neither by itself supplies the weak theorem's finite quotient.

After finite generation, $E(K)$ is a finite [torsion subgroup](../../../../../torsion-subgroup.md) plus a free [abelian group](../../../../../abelian-group.md) of finite rank. The canonical height pairing is positive-definite on the associated real vector space. To justify the latter rather than assuming it, if its nonnegative quadratic form had a real null direction, rounding longer and longer multiples of that direction to lattice points would produce infinitely many points of bounded height: the null-direction cross terms vanish, leaving only uniformly bounded rounding errors. This contradicts Northcott finiteness. Hence the free part is a Euclidean height lattice. Heights can consequently bound point searches, certify independence through positive Gram determinants, and organize the arithmetic complexity of rational points.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
