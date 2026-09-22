<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The central idea of [Galois cohomology of an elliptic curve](../../../../../galois-cohomology-of-an-elliptic-curve.md) is to encode obstructions to dividing rational points, then compare those obstructions over $\mathbb Q$ and its completions. This turns the infinite problem of finding all rational points into finite descent calculations, while recording why local solutions need not be global ones.

Let $G_K=\operatorname{Gal}(\overline K/K)$ for a number field $K$, and regard $E(\overline K)$ as a discrete [Galois module](../../../../../galois-module.md). Then $H^0(K,E)=E(K)$. A continuous [Galois cohomology](../../../../../galois-cohomology.md) one-cocycle is a map $c:G_K\to E(\overline K)$ satisfying

$$
c_{\sigma\tau}=c_\sigma+\sigma c_\tau.
$$

Two cocycles represent the same class in $H^1(K,E)$ if their difference is $\sigma Q-Q$ for some geometric point $Q$. The resulting [Weil–Châtelet group](../../../../../weil-chatelet-group.md) classifies [algebraic-group torsors](../../../../../algebraic-group-torsor.md) under $E$: genus-one curves with an $E$-action, which become copies of $E$ over $\overline K$. Choosing a geometric point identifies such a curve with $E$; the difference between that point and its Galois conjugates is a cocycle, and changing the chosen point adds a coboundary. A torsor class is zero exactly when the curve has a $K$-point. Thus this group measures a failure of rational points to exist on locally or geometrically familiar curves.

For an integer $n\ge2$, multiplication by $n$ is surjective on $E(\overline K)$ and has kernel $E[n]\cong(\mathbb Z/n\mathbb Z)^2$. The [Kummer exact sequence of an elliptic curve](../../../../../kummer-exact-sequence-of-an-elliptic-curve.md) is

$$
0\longrightarrow E[n]\longrightarrow E(\overline K)\xrightarrow{[n]}E(\overline K)\longrightarrow0.
$$

Taking [Galois cohomology](../../../../../galois-cohomology.md) yields

$$
\boxed{0\longrightarrow E(K)/nE(K)\xrightarrow{\delta_K}H^1(K,E[n])\longrightarrow H^1(K,E)[n]\longrightarrow0.}
$$

This sequence has an explicit arithmetic meaning. Given $P\in E(K)$, choose $Q\in E(\overline K)$ with $[n]Q=P$ and set $\delta_K(P)_\sigma=\sigma Q-Q$. Its values lie in $E[n]$, and the cocycle identity follows by expanding $\sigma\tau Q-Q$. Choosing another $Q$ changes it by a coboundary in $E[n]$. Replacing $P$ by $P+[n]R$ with $R\in E(K)$ does not change the class. Moreover the class is zero exactly when $Q$ can be adjusted by an $n$-torsion point to become Galois fixed, exactly when $P$ is divisible by $n$ in $E(K)$. Thus the [Kummer map of an elliptic curve](../../../../../kummer-map-of-an-elliptic-curve.md) is an injection of the quotient actually needed for descent, not merely a formal construction.

For each place $v$ of $K$, repeat this construction over the completion $K_v$. Define the [n-Selmer group](../../../../../n-selmer-group.md) by

$$
\operatorname{Sel}^{(n)}(E/K)=\{c\in H^1(K,E[n]):\operatorname{res}_v(c)\in\delta_{K_v}(E(K_v)/nE(K_v))\text{ for every }v\}.
$$

Every global rational point satisfies these local conditions, so $E(K)/nE(K)$ embeds in the Selmer group. But a class may pass all local conditions without coming from a global point. The [Tate–Shafarevich group](../../../../../tate-shafarevich-group.md) records this obstruction:

$$
\operatorname{Sha}(E/K)=\ker\left(H^1(K,E)\longrightarrow\prod_v H^1(K_v,E)\right).
$$

It consists of torsor classes with points over every completion but potentially none over $K$. The global and local Kummer sequences give the [Selmer exact sequence and rank bound](../../../../../selmer-exact-sequence-and-rank-bound.md)

$$
\boxed{0\longrightarrow E(K)/nE(K)\longrightarrow\operatorname{Sel}^{(n)}(E/K)\longrightarrow\operatorname{Sha}(E/K)[n]\longrightarrow0.}
$$

To verify surjectivity on the right, lift a class of $\operatorname{Sha}[n]$ through the global Kummer sequence. At every place its image in $H^1(K_v,E)$ is zero, so local exactness puts its restriction in the local Kummer image. The lift is therefore Selmer. The kernel on the left is the global Kummer image by global exactness. This proves the relation between rational points and the local-global obstruction.

Finiteness is what makes this framework useful. Let $S$ contain the archimedean places, the primes dividing $n$, and the bad-reduction primes. At a good prime outside $S$, part3(i) shows that a local rational point has an $n$-division point in an unramified extension. Its Kummer class is therefore unramified. Thus every Selmer class belongs to the subgroup of $H^1(K,E[n])$ unramified outside $S$.

Here is the arithmetic finiteness argument, without assuming the full [Mordell-Weil theorem](../../../../../mordell-weil-group.md). Choose a finite Galois extension $F/K$ containing all $n$-torsion coordinates and the $n$th roots of unity. Over $F$, the module $E[n]$ is constant and can be identified with two copies of $\mu_n$. [Kummer theory](../../../../../kummer-theory.md) identifies its first cohomology with two copies of $F^\times/F^{\times n}$. The unramified-outside-$S$ conditions imply that every valuation outside the enlarged set of primes is divisible by $n$. The resulting [S-unramified power class group](../../../../../s-unramified-power-class-group.md) fits into

$$
0\longrightarrow\mathcal O_{F,S}^{\times}/(\mathcal O_{F,S}^{\times})^n
\longrightarrow F(S,n)\longrightarrow\operatorname{Cl}(\mathcal O_{F,S})[n]\longrightarrow0.
$$

For the last map, divide the outside-$S$ principal divisor by $n$ and take its ideal class. Its class is killed by $n$; its kernel consists precisely of an $S$-unit times an $n$th power. The [S-unit group](../../../../../s-unit-group.md) is finitely generated: its valuations at the finite primes in $S$ map it into $\mathbb Z^{|S_{\rm fin}|}$, with kernel the ordinary units. The [Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md) makes that kernel finitely generated, and every subgroup of this finite-rank free abelian group is finitely generated. Thus the first term is finite. Finiteness of the [ideal class group](../../../../../ideal-class-group.md) makes the last term finite. The kernel of restriction from $K$ to $F$ is finite by the [inflation-restriction exact sequence](../../../../../inflation-restriction-exact-sequence.md) with finite module $E[n]$ and finite quotient $\operatorname{Gal}(F/K)$. Hence the Selmer group is finite, as is $E(K)/nE(K)$. This proves the [Weak Mordell-Weil theorem](../../../../../weak-mordell-weil-theorem.md) cohomologically and also proves finiteness of $\operatorname{Sha}[n]$, without asserting finiteness of the whole Tate–Shafarevich group.

For $K=\mathbb Q$, combine this finite quotient with a [height descent](../../../../../height-descent-lemma.md). Choose finitely many representatives $R_i$ for $E(\mathbb Q)/2E(\mathbb Q)$, and put $H=\max_i\widehat h(R_i)$, using the nonnegative [canonical height of an elliptic curve](../../../../../canonical-height-of-an-elliptic-curve.md). Its [height parallelogram identity](../../../../../height-parallelogram-identity.md) gives $\widehat h(P-R_i)\le2\widehat h(P)+2\widehat h(R_i)$. Thus if $P=2Q+R_i$,

$$
\widehat h(Q)=\frac14\widehat h(P-R_i)\le\frac12\widehat h(P)+\frac H2.
$$

Iteration eventually brings the height below $H+1$. The [Northcott theorem](../../../../../northcott-theorem.md), together with the bounded difference between canonical and naive heights, makes that terminal set finite. Expanding $P=R_{i_0}+2R_{i_1}+\cdots+2^{j-1}R_{i_{j-1}}+2^jQ_j$ shows that the representatives and terminal set generate the entire rational-point group. This is the [canonical-height proof of Mordell-Weil finite generation](../../../../../canonical-height-proof-of-mordell-weil-finite-generation.md): cohomology supplies finite quotients, and height supplies the descent needed to obtain generators.

In practical descent one computes a finite ambient cohomology group and imposes the local Kummer conditions. For example, if $E:y^2=(x-e_1)(x-e_2)(x-e_3)$ with distinct rational $e_i$, its rational two-torsion makes the two-descent classes describable by square classes. The coordinate function $x-e_i$ has [principal divisor](../../../../../principal-divisor-on-an-algebraic-curve.md) $2(T_i)-2(O)$, where $T_i=(e_i,0)$ is a two-torsion point. The [Weil pairing](../../../../../weil-pairing.md) identifies the corresponding two-torsion characters with square-class Kummer coordinates. For a point with $x\ne e_i$, its Kummer class is represented by

$$
(x-e_1,\ x-e_2,\ x-e_3)\in(\mathbb Q^\times/\mathbb Q^{\times2})^3,
$$

with product one because it is represented by $y^2$. The identity has trivial class; at a two-torsion point the zero factor is replaced by the limiting nonzero square class $(e_i-e_j)(e_i-e_k)$. A representative triple $(d_1,d_2,d_3)$ with square product gives a covering described by

$$
d_1u_1^2-d_2u_2^2=(e_2-e_1)t^2,\qquad
d_2u_2^2-d_3u_3^2=(e_3-e_2)t^2.
$$

For $t\ne0$, a rational point on the covering gives $x=e_1+d_1(u_1/t)^2$ and recovers $y$ from the product. Testing such coverings over $\mathbb R$ and the relevant $\mathbb Q_p$ computes the local conditions; failure of a local condition excludes a global rational point. Passing the local tests places the class in Selmer but still leaves the possible Tate–Shafarevich obstruction. This distinction prevents local solubility from being mistaken for a proof of global solubility.

Finally, writing $E(\mathbb Q)\cong\mathbb Z^r\oplus T$ after finite generation, for a prime $\ell$ the exact sequence gives

$$
\dim_{\mathbb F_\ell}\operatorname{Sel}^{(\ell)}(E/\mathbb Q)
=r+\dim_{\mathbb F_\ell}E(\mathbb Q)[\ell]+\dim_{\mathbb F_\ell}\operatorname{Sha}(E/\mathbb Q)[\ell].
$$

Consequently a Selmer computation bounds the [rank of an elliptic curve](../../../../../rank-of-an-elliptic-curve.md) above; independent rational points bound it below, and a [canonical height pairing](../../../../../canonical-height-pairing.md) can certify their independence. When the bounds agree the rank is proved, but a further [Mordell-Weil saturation](../../../../../mordell-weil-saturation.md) calculation is needed to know that the found points generate the full group. For a general [isogeny of elliptic curves](../../../../../isogeny-of-elliptic-curves.md) $\varphi:E\to E'$, the same argument starts from $0\to E[\varphi]\to E(\overline K)\xrightarrow{\varphi}E'(\overline K)\to0$, producing an [isogeny Selmer group](../../../../../isogeny-selmer-group.md) and often a smaller descent calculation. **Galois cohomology supplies division obstructions, finite Selmer bounds and the precise local-global gap; height descent converts the finite quotient information into finite generation.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
