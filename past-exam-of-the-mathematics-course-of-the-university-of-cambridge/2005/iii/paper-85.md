# Paper 85

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper85.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper85.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 85](paper-85.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Take rings and modules to be unital. Let $J_\ell$ denote the intersection of the [maximal left ideals](../../../associative-algebra.md#maximal-left-ideal). For each nonzero vector $v$ of a [simple module](../../../module-theory.md#irreducible-module) $M$ on the left, the map $R\to M$, $r\mapsto rv$, is onto and its kernel is a [maximal left ideal](../../../associative-algebra.md#maximal-left-ideal). Consequently $J_\ell$ annihilates every [simple module](../../../module-theory.md#irreducible-module) on the left. Conversely, annihilating $R/L$ forces an element to belong to the [maximal left ideal](../../../associative-algebra.md#maximal-left-ideal) $L$. Thus

$$
J_\ell=\bigcap_{M\text{ simple left}}\operatorname{Ann}_R(M),
$$

which shows that $J_\ell$ is a two-sided [ideal](../../../commutative-algebra.md#ideal).

For $j\in J_\ell$ and $r\in R$, the [left ideal](../../../associative-algebra.md#left-ideal) $R(1-rj)$ cannot be proper: a containing [maximal left ideal](../../../associative-algebra.md#maximal-left-ideal) would also contain $rj$ and hence $1$. Therefore $u(1-rj)=1$ for some $u\in R$. Here $u=1+urj$ also differs from $1$ by an element of $J_\ell$, so it too has a left inverse $v$. Multiplying the first equality by $v$ gives $1-rj=v$; hence $(1-rj)u=1$. We have proved that $1-rj$ is a [unit](../../../algebra.md#unit-in-a-ring), not just left invertible.

The identity

$$
(1-ba)^{-1}=1+b(1-ab)^{-1}a
$$

is verified by multiplying on either side, using $(1-ab)^{-1}(1-ab)=(1-ab)(1-ab)^{-1}=1$. It implies that $1-jr$ is a [unit](../../../algebra.md#unit-in-a-ring) as well. If $j$ were outside a [maximal right ideal](../../../associative-algebra.md#maximal-right-ideal) $I$, then $I+jR=R$, so $1-jr\in I$ for some $r$. A proper [right ideal](../../../associative-algebra.md#right-ideal) cannot contain a [unit](../../../algebra.md#unit-in-a-ring), giving a contradiction. Thus $J_\ell$ belongs to every [maximal right ideal](../../../associative-algebra.md#maximal-right-ideal). Applying the same argument to the [opposite ring](../../../commutative-algebra.md#opposite-ring) proves the reverse inclusion. This proves the [Jacobson radical is independent of handedness](../../../noncommutative-algebra.md#jacobson-radical-is-independent-of-handedness):

$$
\boxed{J(R)=\bigcap_{L\text{ maximal left}}L=\bigcap_{I\text{ maximal right}}I.}
$$

For the zero ring the intersections are interpreted as the whole ring, so the equality remains valid.

If a two-sided [ideal](../../../commutative-algebra.md#ideal) $N$ satisfies $N^m=0$, then for $x\in N$ and $r\in R$, $(rx)^m=0$. The finite [geometric series](../../../real-analysis.md#geometric-series) $\sum_{i=0}^{m-1}(rx)^i$ inverts $1-rx$. The [unit criterion for the Jacobson radical](../../../noncommutative-algebra.md#unit-criterion-for-the-jacobson-radical), also proved above by the maximal-ideal argument, gives **$N\subseteq J(R)$**. This assertion concerns a [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal); arbitrary [nilpotent elements](../../../commutative-algebra.md#nilpotent) of a noncommutative ring need not lie in its [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical).

For the [formal power series ring](../../../commutative-algebra.md#formal-power-series) over the [p-adic integers](../../../number-theory.md#p-adic-integer), a series $f=\sum_{i\ge0}a_it^i$ is a [unit](../../../algebra.md#unit-in-a-ring) exactly when $a_0$ is a [unit](../../../algebra.md#unit-in-a-ring) of $\mathbb Z_p$. Necessity follows by comparing constant coefficients. If $a_0$ is invertible, construct the inverse recursively by $b_0=a_0^{-1}$ and $b_m=-a_0^{-1}\sum_{i=1}^m a_ib_{m-i}$. Therefore the nonunits are exactly the series whose constant coefficient lies in $p\mathbb Z_p$. They form the unique maximal [ideal](../../../commutative-algebra.md#ideal) $(p,t)$, and the quotient is $\mathbb F_p$. Hence

$$
\boxed{J(\mathbb Z_p[[t]])=(p,t).}
$$

## 2

↑ **Parent:** [Paper 85](paper-85.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The variable $t$ is central. To prove the [leading-coefficient proof for a central polynomial extension](../../../noncommutative-algebra.md#leading-coefficient-proof-for-a-central-polynomial-extension), let $I$ be any [right ideal](../../../associative-algebra.md#right-ideal) of $R[t]$ and set

$$
L_d=\left\{a_d:\sum_{i=0}^d a_it^i\in I\right\}\subseteq R.
$$

Zero leading coefficients are allowed. Addition and right multiplication by constants show that $L_d$ is a [right ideal](../../../associative-algebra.md#right-ideal). Multiplication by $t$ gives $L_d\subseteq L_{d+1}$. Since $R$ is a [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring), this chain stabilizes, say at $L_N$, and each $L_d$ for $d\le N$ has finitely many generators $a_{dj}$. Choose $f_{dj}\in I$ of degree at most $d$ lifting these coefficients.

These finitely many polynomial lifts generate $I$ on the right. Indeed, for $f\in I$ of degree $m$, let $d=\min(m,N)$. Write its leading coefficient as $\sum_j a_{dj}r_j$. Then

$$
f-\sum_j f_{dj}\,r_jt^{m-d}
$$

belongs to $I$ and has degree less than $m$, because $L_m=L_d$ when $m>N$. Induction on degree reduces $f$ to a right linear combination of the chosen lifts. This proves finite generation of every [right ideal](../../../associative-algebra.md#right-ideal), and hence

$$
\boxed{R\text{ right Noetherian}\Longrightarrow R[t]\text{ right Noetherian}.}
$$

Centrality matters: it is what permits the displayed leading-coefficient cancellation without twisting the coefficients.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the degree-one convention implicit in this enveloping-algebra assertion: a [degree-one almost commutative algebra](../../../module-theory.md#degree-one-almost-commutative-algebra) has $F_0R=k$, a finite-dimensional $F_1R$ containing $1$ which generates $R$, and commutative [associated graded ring](../../../commutative-algebra.md#associated-graded-ring). Taking the leading symbol of a [commutator](../../../lie-algebra.md#commutator) gives

$$
[F_iR,F_jR]\subseteq F_{i+j-1}R,
$$

in particular $[F_1R,F_1R]\subseteq F_1R$. Thus $\mathfrak g=F_1R$, equipped with $[u,v]=uv-vu$, is a finite-dimensional [Lie algebra](../../../lie-algebra.md). Bilinearity and antisymmetry are immediate, and expanding the three nested [commutators](../../../lie-algebra.md#commutator) proves the [Jacobi identity](../../../lie-algebra.md#jacobi-identity).

Its inclusion into the associative [algebra](../../../algebra.md) $R$ is a [Lie algebra homomorphism](../../../lie-algebra.md#lie-algebra-homomorphism). The [universal enveloping algebra](../../../lie-algebra.md#universal-enveloping-algebra) is $T(\mathfrak g)$ modulo the relations $u\otimes v-v\otimes u-[u,v]$. Sending the tensor generators to their elements of $R$ kills these relations and gives an [algebra homomorphism](../../../algebra.md#algebra-homomorphism-over-a-field) $U(\mathfrak g)\to R$. It is surjective because $F_1R$ generates $R$. Therefore

$$
\boxed{R\cong U(\mathfrak g)/\ker(U(\mathfrak g)\to R),\qquad \dim_k\mathfrak g<\infty.}
$$

The vector $1\in F_1R$ is retained as a central [Lie algebra](../../../lie-algebra.md) generator and maps to the associative identity; its corresponding relation in the kernel is that generator minus $1_{U(\mathfrak g)}$. One should not first replace $F_1R$ by $F_1R/k1$, since [commutators](../../../lie-algebra.md#commutator) of generators can be nonzero scalars.

Terminology is important here. Merely requiring a commutative finitely generated [associated graded ring](../../../commutative-algebra.md#associated-graded-ring) for an arbitrary weighted [filtration](../../../stochastic-process.md#filtration-probability-theory) is a broader definition of [almost commutative algebra](../../../module-theory.md#almost-commutative-algebra); it does not supply the finite-dimensional bracket-closed first step used in this argument. The degree-one assumptions make the requested enveloping presentation precise. The Noetherianity in part (b) also follows directly under the broader finite-generation convention.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Give $U(\mathfrak g)$ its degree [filtration](../../../stochastic-process.md#filtration-probability-theory). The [Poincaré-Birkhoff-Witt theorem](../../../lie-algebra.md#poincare-birkhoff-witt-theorem) identifies its [associated graded ring](../../../commutative-algebra.md#associated-graded-ring) with $\operatorname{Sym}_k\mathfrak g$, a [polynomial ring](../../../commutative-algebra.md#polynomial-ring) in $\dim_k\mathfrak g$ variables. The [Hilbert basis theorem](../../../algebra.md#hilbert-basis-theorem) makes this graded [algebra](../../../algebra.md) [Noetherian](../../../algebra.md#noetherian-ring) on both sides.

Here is the required transfer, including why a finite list of symbols gives actual generators. For a [right ideal](../../../associative-algebra.md#right-ideal) $I$ of a nonnegatively filtered [ring](../../../commutative-algebra.md#ring) $A$, its induced graded [ideal](../../../commutative-algebra.md#ideal) $\operatorname{gr}I$ is a homogeneous [right ideal](../../../associative-algebra.md#right-ideal) of $\operatorname{gr}A$. Choose finite homogeneous generators and lift them to $u_1,\ldots,u_m\in I$. For $u\in I$ of degree $d$, express its leading symbol as a graded right linear combination of these symbols, using homogeneous coefficients of complementary degrees. Lift the coefficients to $A$ and subtract the corresponding $\sum_i u_ia_i$. The remainder has degree strictly below $d$. Induction, terminating because degrees are nonnegative, proves $I=\sum_i u_iA$. The identical argument with coefficients on the left treats [left ideals](../../../associative-algebra.md#left-ideal).

This [ascending filtered-graded transfer of Noetherianity](../../../module-theory.md#ascending-filtered-graded-transfer-of-noetherianity) proves that $U(\mathfrak g)$ is right and left [Noetherian](../../../algebra.md#noetherian-ring). A [quotient ring](../../../commutative-algebra.md#quotient-ring) inherits either property: pull an ascending ideal chain back to the original [ring](../../../commutative-algebra.md#ring), or take images of ideal generators. Part (a) therefore gives **$R$ right and left Noetherian**. Alternatively, under the broader [almost commutative algebra](../../../module-theory.md#almost-commutative-algebra) convention, its commutative finitely generated [associated graded ring](../../../commutative-algebra.md#associated-graded-ring) is directly a quotient of a finite-variable [polynomial ring](../../../commutative-algebra.md#polynomial-ring), and the same leading-symbol argument proves the conclusion.

## 3

↑ **Parent:** [Paper 85](paper-85.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A right [Ore localization](../../../noncommutative-algebra.md#ore-localization) at $S$ is a unital homomorphism $\iota:R\to Q$ such that every $\iota(s)$, $s\in S$, is a [unit](../../../algebra.md#unit-in-a-ring), every element of $Q$ is $\iota(r)\iota(s)^{-1}$, and

$$
\ker\iota=\{r\in R:rt=0\text{ for some }t\in S\}.
$$

Equivalently, the usual fraction construction has this zero criterion and is universal among homomorphisms that invert $S$. Injectivity is required only when the denominators are [regular elements of a ring](../../../noncommutative-algebra.md#regular-element-of-a-ring). If $0\in S$, every homomorphism inverting $S$ has zero target; this is the degenerate zero-ring localization. For a nonzero localization we require $0\notin S$.

The necessary and sufficient conditions are that $S$ be a [right denominator set](../../../noncommutative-algebra.md#right-denominator-set):

- For $r\in R$ and $s\in S$, there are $t\in S$ and $b\in R$ with $rt=sb$; this is the [right Ore condition](../../../noncommutative-algebra.md#right-ore-condition).
- If $sr=0$ with $s\in S$, there is $t\in S$ with $rt=0$; this is right reversibility.

For necessity, write the element $\iota(s)^{-1}\iota(r)$ as $\iota(b)\iota(t)^{-1}$. Multiplying by $\iota(s)$ on the left and $\iota(t)$ on the right gives $\iota(rt-sb)=0$. The zero criterion supplies $u\in S$ with $(rt-sb)u=0$. Hence $r(tu)=s(bu)$, the [right Ore condition](../../../noncommutative-algebra.md#right-ore-condition) in $R$, not merely an equality of images in $Q$. Also $sr=0$ makes $\iota(r)=0$ because $\iota(s)$ is invertible, and the zero criterion gives $rt=0$. This proves both necessities.

The sufficiency is the [Ore theorem](../../../noncommutative-algebra.md#ore-theorem) for denominator sets. Concretely, right fractions can be represented by $(r,s)$; a common-denominator equality has $su=tv\in S$ and $ru=r'v$ for suitable $u,v\in R$. The two conditions make the induced fraction equivalence transitive and make addition and multiplication well defined; the zero fraction is exactly the kernel displayed above. The requested direction of the theorem was necessity, for which the complete argument has just been given.

For a [right Noetherian domain](../../../noncommutative-algebra.md#right-noetherian-domain), any two nonzero principal [right ideals](../../../associative-algebra.md#right-ideal) intersect. To see this without using the desired localization, suppose $bR\cap aR=0$ with $a,b\ne0$. The sum

$$
bR+abR+a^2bR+\cdots
$$

is direct: reduce a finite relation modulo $aR$ to get its first summand zero, then cancel $a$ in the [noncommutative domain](../../../noncommutative-algebra.md#noncommutative-domain) and repeat. Every summand is nonzero, so the finite partial sums form a strictly ascending chain of [right ideals](../../../associative-algebra.md#right-ideal), contradicting the [ascending chain condition](../../../algebra.md#ascending-chain-condition). A nonzero intersection $rR\cap sR$ thus provides $rt=sb\ne0$, with $t\ne0$. This is the [right Ore condition](../../../noncommutative-algebra.md#right-ore-condition) for $S=R\setminus\{0\}$. Reversibility is automatic in a [noncommutative domain](../../../noncommutative-algebra.md#noncommutative-domain), and the zero criterion makes the map injective. The localization is a [division ring](../../../commutative-algebra.md#division-ring), since a nonzero $rs^{-1}$ has inverse $sr^{-1}$.

The [Goldie theorem](../../../noncommutative-algebra.md#goldie-s-theorem) states that a [semiprime ring](../../../noncommutative-algebra.md#semiprime-ring) has a semisimple Artinian [classical right ring of quotients](../../../noncommutative-algebra.md#classical-right-ring-of-quotients) if and only if it has finite right [uniform dimension](../../../module-theory.md#uniform-dimension) and satisfies the [ascending chain condition](../../../algebra.md#ascending-chain-condition) on [right annihilators](../../../module-theory.md#right-annihilator). A [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring) satisfies the annihilator condition because [right annihilators](../../../module-theory.md#right-annihilator) are [right ideals](../../../associative-algebra.md#right-ideal). Its right regular [module](../../../module-theory.md#module-mathematics) has finite [uniform dimension](../../../module-theory.md#uniform-dimension): an infinite direct sum of nonzero submodules would give a strictly ascending chain of finite partial sums. A [prime ring](../../../noncommutative-algebra.md#prime-ring) is [semiprime](../../../number-theory.md#semiprime), so the theorem applies to a prime [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring) $R$.

To obtain a single matrix-ring factor, not just a finite product, prove that its quotient $Q$ is prime. A nonzero two-sided [ideal](../../../commutative-algebra.md#ideal) $I\subseteq Q$ contains a nonzero fraction $rs^{-1}$ and hence the nonzero element $r=(rs^{-1})s\in I\cap R$. The same holds for any other nonzero [ideal](../../../commutative-algebra.md#ideal) $K$. Since $R$ is prime, $(I\cap R)(K\cap R)\ne0$, so $IK\ne0$. Thus $Q$ is prime. The [Artin–Wedderburn theorem](../../../associative-algebra.md#artin-wedderburn-theorem) gives a finite product of matrix rings over [division rings](../../../commutative-algebra.md#division-ring); primeness excludes two different nonzero factors with zero product. This proves the [prime classical quotient of a prime right Goldie ring](../../../noncommutative-algebra.md#prime-classical-quotient-of-a-prime-right-goldie-ring):

$$
\boxed{Q_{\mathrm{cl}}^r(R)\cong M_n(D)\quad\text{for a division ring }D.}
$$

For the requested counterexample to Noetherianity, take $R=k[x_1,x_2,\ldots]$. It is a commutative [integral domain](../../../commutative-algebra.md#integral-domain) and has its [field of fractions](../../../commutative-algebra.md#field-of-fractions) as its [classical right ring of quotients](../../../noncommutative-algebra.md#classical-right-ring-of-quotients). But $(x_1)\subsetneq(x_1,x_2)\subsetneq\cdots$ is a strictly ascending ideal chain: evaluation at $x_1=\cdots=x_m=0$ shows $x_{m+1}$ is not in the preceding [ideal](../../../commutative-algebra.md#ideal). Therefore existence of a classical quotient does **not** imply right Noetherianity.

## 4

↑ **Parent:** [Paper 85](paper-85.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use the [descending chain condition](../../../algebra.md#descending-chain-condition) on the finite intersections of [maximal right ideals](../../../associative-algebra.md#maximal-right-ideal). It gives a minimal such intersection $K=M_1\cap\cdots\cap M_r$. Intersecting $K$ with any other [maximal right ideal](../../../associative-algebra.md#maximal-right-ideal) cannot decrease it, by minimality. Thus $K$ lies in every [maximal right ideal](../../../associative-algebra.md#maximal-right-ideal), and $K=J(R)$. When $J(R)=0$, the diagonal map

$$
R_R\longrightarrow\bigoplus_{i=1}^rR/M_i,\qquad a\longmapsto(a+M_i)_i
$$

is injective, and each summand on the right is a [simple module](../../../module-theory.md#irreducible-module).

For completeness, a submodule $N$ of a finite direct sum of [simple modules](../../../module-theory.md#irreducible-module) is semisimple. Induct on the number of summands. For $S\oplus T$ with $S$ simple, $N\cap S$ is either $0$ or $S$. In the first case projection into $T$ identifies $N$ with a submodule of $T$, so induction applies. In the second case subtracting the $S$ coordinate shows $N=S\oplus(N\cap T)$, and induction again applies. This also shows finite [module length](../../../module-theory.md#length-of-a-module). Apply it to the image of the diagonal map to obtain

$$
\boxed{J(R)=0\text{ and }R\text{ right Artinian}\Longrightarrow R_R\text{ semisimple}.}
$$

This is the [semisimplicity of a right Artinian ring with zero radical](../../../noncommutative-algebra.md#semisimplicity-of-a-right-artinian-ring-with-zero-radical). It does not assume right Noetherianity in order to prove it.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The descending powers $J\supseteq J^2\supseteq\cdots$ stabilize because they are [right ideals](../../../associative-algebra.md#right-ideal). Choose $m\ge1$ with $J^m=J^{m+1}$ and put $I=J^m$. Then $I=J^{2m}=I^2$.

Suppose $I\ne0$. Among the [right ideals](../../../associative-algebra.md#right-ideal) $K$ such that $KI\ne0$, choose a minimal one; the set is nonempty since $RI=I\ne0$. The [right ideal](../../../associative-algebra.md#right-ideal) $KI$ lies in $K$, and $(KI)I=KI^2=KI\ne0$, so minimality forces $KI=K$. Choose $k\in K$ with $kI\ne0$. Then $(kR)I=kI\ne0$, and $kR\subseteq K$, so the same minimality gives $K=kR$.

Since $K=KI$ and $I\subseteq J$, its generator satisfies $k=\sum_\nu kr_\nu i_\nu=kj$ for an element $j=\sum_\nu r_\nu i_\nu\in J$. Thus $k(1-j)=0$. The [unit criterion for the Jacobson radical](../../../noncommutative-algebra.md#unit-criterion-for-the-jacobson-radical) makes $1-j$ invertible, implying $k=0$, contrary to $kI\ne0$. Therefore $I=0$, and

$$
\boxed{J(R)^m=0.}
$$

The [minimal-right-ideal proof of radical nilpotence](../../../noncommutative-algebra.md#minimal-right-ideal-proof-of-radical-nilpotence) is important here: one cannot apply the finite-generator form of [Nakayama lemma](../../../mathematics.md#nakayama-lemma) directly to $J^m$ before proving it finitely generated. We made a suitable auxiliary [right ideal](../../../associative-algebra.md#right-ideal) cyclic before using the unit argument.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Maximal [right ideals](../../../associative-algebra.md#right-ideal) of $R/J$ correspond to [maximal right ideals](../../../associative-algebra.md#maximal-right-ideal) of $R$, all of which contain $J$. Their intersection in the quotient is zero. Hence $R/J$ is a [right Artinian ring](../../../noncommutative-algebra.md#right-artinian-ring) with zero [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical), and part (a) makes it semisimple.

Part (b) gives the finite radical filtration

$$
R\supseteq J\supseteq J^2\supseteq\cdots\supseteq J^m=0.
$$

Each factor $J^i/J^{i+1}$ is annihilated by $J$, so it is a right [module](../../../module-theory.md#module-mathematics) over $R/J$. Every [module](../../../module-theory.md#module-mathematics) over a semisimple [ring](../../../commutative-algebra.md#ring) is semisimple: a free [module](../../../module-theory.md#module-mathematics) is a direct sum of simple summands of copies of the regular [module](../../../module-theory.md#module-mathematics), and a quotient of a semisimple [module](../../../module-theory.md#module-mathematics) is again semisimple, because the images of its simple summands are either zero or simple and span the quotient. A maximal independent family of these simple images spans: any simple image not contained in the sum intersects it trivially and could be added. Each factor is also [Artinian](../../../algebra.md#artinian-ring), as a subquotient of $R_R$. A semisimple [Artinian module](../../../module-theory.md#artinian-module) has only finitely many simple summands, since an infinite direct sum would give a descending chain by successively deleting summands. Consequently every factor has finite [module length](../../../module-theory.md#length-of-a-module).

Concatenating composition series of these finitely many factors makes $R_R$ a [module](../../../module-theory.md#module-mathematics) of finite [module length](../../../module-theory.md#length-of-a-module). Such a [module](../../../module-theory.md#module-mathematics) satisfies both chain conditions, since every strict change consumes a positive amount of length. Therefore **$R$ is right Noetherian**. This is the [Hopkins-Levitzki theorem](../../../noncommutative-algebra.md#hopkins-levitzki-theorem), obtained from the two preceding results rather than invoked in their proofs.

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $K=k(z)$, where $z$ is an indeterminate, and form the [right Artinian triangular ring that is not left Noetherian](../../../noncommutative-algebra.md#right-artinian-triangular-ring-that-is-not-left-noetherian)

$$
\boxed{T=\begin{pmatrix}k&K\\0&K\end{pmatrix}.}
$$

Multiplication uses the natural $k$–$K$ bimodule structure on the upper-right entry. With the two diagonal [idempotents](../../../commutative-algebra.md#idempotent) $e_1,e_2$, the right regular [module](../../../module-theory.md#module-mathematics) is $e_1T\oplus e_2T$. The off-diagonal submodule of $e_1T$ is one-dimensional over the bottom-right [field](../../../algebra.md#field) $K$, hence simple. Its quotient is one-dimensional over the top-left [field](../../../algebra.md#field) $k$, hence simple. Also $e_2T$ is a simple right [module](../../../module-theory.md#module-mathematics) over $K$. Thus $T_T$ has a composition series of length three, and in particular $T$ is right [Artinian](../../../algebra.md#artinian-ring).

On the left, multiplication of an off-diagonal matrix gives

$$
\begin{pmatrix}a&m\\0&b\end{pmatrix}
\begin{pmatrix}0&u\\0&0\end{pmatrix}
=\begin{pmatrix}0&au\\0&0\end{pmatrix}.
$$

Every $k$-subspace $U\subseteq K$ therefore yields a [left ideal](../../../associative-algebra.md#left-ideal) of off-diagonal matrices with entries in $U$. The subspaces $U_m=\operatorname{span}_k\{1,z,\ldots,z^m\}$ are strictly increasing because $z$ is transcendental. Their associated [left ideals](../../../associative-algebra.md#left-ideal) violate the [ascending chain condition](../../../algebra.md#ascending-chain-condition). Hence **$T$ is not left Noetherian**, even though it is right Artinian and right Noetherian.

## 5

↑ **Parent:** [Paper 85](paper-85.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

In a commutative [ring](../../../commutative-algebra.md#ring), if $x^m=0$, then the principal [ideal](../../../commutative-algebra.md#ideal) $(x)$ satisfies $(x)^m=0$. Thus a [semiprime ring](../../../noncommutative-algebra.md#semiprime-ring) has no nonzero [nilpotent elements](../../../commutative-algebra.md#nilpotent). Conversely, if $I^m=0$ for an [ideal](../../../commutative-algebra.md#ideal) $I$, then every $x\in I$ satisfies $x^m=0$; absence of nonzero [nilpotent elements](../../../commutative-algebra.md#nilpotent) forces $I=0$. Hence **commutative semiprimeness is exactly reducedness**.

For a [prime ideal](../../../commutative-algebra.md#prime-ideal) $P$, let $S=R\setminus P$. Every [ideal](../../../commutative-algebra.md#ideal) $I$ of $R_P=S^{-1}R$ is the extension of its contraction $I^c$: if $r/s\in I$, multiply by the [unit](../../../algebra.md#unit-in-a-ring) $s/1$ to get $r/1\in I$, so $r\in I^c$. If $R$ is [Noetherian](../../../algebra.md#noetherian-ring), write $I^c=(r_1,\ldots,r_m)$; their images generate $I$. This proves that $R_P$ is [Noetherian](../../../algebra.md#noetherian-ring).

The extended [ideal](../../../commutative-algebra.md#ideal) $PR_P$ is proper. Indeed $1=p/s$ would imply $u(s-p)=0$ for some $u\notin P$, and then $us=up\in P$, contradicting primeness and $u,s\notin P$. A fraction with numerator outside $P$ is invertible, with inverse $s/r$. A fraction with numerator in $P$ lies in the proper [ideal](../../../commutative-algebra.md#ideal) $PR_P$ and cannot be invertible. Thus the nonunits are precisely $PR_P$, making it the unique maximal [ideal](../../../commutative-algebra.md#ideal). Therefore

$$
\boxed{R_P\text{ is a Noetherian local ring with maximal ideal }PR_P.}
$$

To prove reducedness is detected by prime localizations, let $x$ be a [nilpotent element](../../../commutative-algebra.md#nilpotent) of $R$. Its image in every $R_Q$ is zero because these localizations are semiprime, hence reduced. If $x\ne0$, its [annihilator](../../../module-theory.md#annihilator-ring-theory) $\operatorname{Ann}(x)$ is a proper [ideal](../../../commutative-algebra.md#ideal); choose a maximal [ideal](../../../commutative-algebra.md#ideal) $Q$ containing it. The zero criterion for [localization](../../../commutative-algebra.md#localization-of-a-ring) says $x/1=0$ in $R_Q$ only if $sx=0$ for some $s\notin Q$, which would put $s$ in $\operatorname{Ann}(x)\subseteq Q$, a contradiction. Hence $x=0$, and $R$ is semiprime. This argument does not need Noetherianity.

Primeness is not detected in the same way. Take **$R=k\times k$**. Its two [prime ideals](../../../commutative-algebra.md#prime-ideal) are $P_1=0\times k$ and $P_2=k\times0$, and its corresponding localizations are both isomorphic to the [field](../../../algebra.md#field) $k$. To see these are all the [prime ideals](../../../commutative-algebra.md#prime-ideal), the orthogonal [idempotents](../../../commutative-algebra.md#idempotent) $e_1,e_2$ have product zero, so a [prime ideal](../../../commutative-algebra.md#prime-ideal) contains one of them and is then the kernel of the other projection. Both localizations are prime [rings](../../../commutative-algebra.md#ring), but $R$ is not prime: $e_1,e_2\ne0$ and $e_1e_2=0$.

## 6

↑ **Parent:** [Paper 85](paper-85.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

This part proves $(c)\Rightarrow(a)$. Write the [Weyl algebra](../../../noncommutative-algebra.md#weyl-algebra) generators as $x_1,\ldots,x_n,D_1,\ldots,D_n$, with $[D_i,x_j]=\delta_{ij}$ and the other generator [commutators](../../../lie-algebra.md#commutator) zero. The ordered [monomials](../../../polynomial.md#monomial) $x^\alpha D^\beta$ form a [basis](../../../vector-space.md#basis) over any [field](../../../algebra.md#field): one may construct the [algebra](../../../algebra.md) by successively adjoining the commuting derivations $D_i$ to $k[x_1,\ldots,x_n]$, with multiplication $D_if=fD_i+\partial f/\partial x_i$, obtaining unique ordered forms. This also makes $A_n(k)$ infinite-dimensional for $n\ge1$.

Assume $\operatorname{char}k=0$ and let $I$ be a nonzero two-sided [ideal](../../../commutative-algebra.md#ideal). Choose a nonzero element $a=\sum c_{\alpha\beta}x^\alpha D^\beta\in I$, and a nonzero term of maximal total degree, say $(\alpha_0,\beta_0)$. The relations give

$$
[D_i,x^\alpha D^\beta]=\alpha_i x^{\alpha-e_i}D^\beta,\qquad
[x_i,x^\alpha D^\beta]=-\beta_i x^\alpha D^{\beta-e_i}.
$$

Apply $(\operatorname{ad}D)^{\alpha_0}(\operatorname{ad}x)^{\beta_0}$ to $a$. Every lower-degree term vanishes. A term of the same degree survives only if all its exponents dominate $(\alpha_0,\beta_0)$, which forces equality. Thus the resulting element of $I$ is

$$
(-1)^{|\beta_0|}\alpha_0!\beta_0!c_{\alpha_0\beta_0}\ne0.
$$

The factorials are nonzero in characteristic zero. This is a nonzero [scalar](../../../vector-space.md#scalar), so $1\in I$ and $I=A_n(k)$. Therefore **$A_n(k)$ is simple in characteristic zero**. This [scalar extraction by iterated Weyl commutators](../../../associative-algebra.md#scalar-extraction-by-iterated-weyl-commutators) supplies the full simplicity proof.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

This part proves $(a)\Rightarrow(b)$. If $M\ne0$ were a finite-dimensional unital [module](../../../module-theory.md#module-mathematics), its action would give a homomorphism

$$
A_n(k)\longrightarrow\operatorname{End}_k(M).
$$

The kernel is a two-sided [ideal](../../../commutative-algebra.md#ideal) and is proper because the identity acts as the identity on $M$. A [simple ring](../../../commutative-algebra.md#simple-ring) therefore makes the homomorphism injective. This is impossible: $A_n(k)$ has the infinitely many linearly independent ordered [monomials](../../../polynomial.md#monomial) established in part (a), whereas the endomorphism [algebra](../../../algebra.md) has dimension $(\dim_kM)^2$. Thus simplicity excludes every nonzero finite-dimensional [module](../../../module-theory.md#module-mathematics).

There is also a direct characteristic-zero check: the relation $[D_1,x_1]=1$ acts as a matrix identity. Taking its [trace](../../../linear-algebra.md#matrix-trace) gives $0=\dim_kM$ in $k$. In characteristic zero this forces $M=0$. This agrees with the [Weyl algebra has no nonzero finite-dimensional modules](../../../noncommutative-algebra.md#weyl-algebra-has-no-nonzero-finite-dimensional-modules) criterion, but the injectivity argument proves the requested implication without presupposing characteristic zero.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For the contrapositive of $(b)\Rightarrow(c)$, suppose $\operatorname{char}k=p>0$. Consider

$$
M=k[x_1,\ldots,x_n]/(x_1^p,\ldots,x_n^p).
$$

Let $x_i$ act by multiplication and $D_i$ by formal differentiation. Differentiation preserves the defining [ideal](../../../commutative-algebra.md#ideal), since $D_j(x_i^pf)=x_i^pD_jf$ in characteristic $p$. The relations $[D_i,x_j]=\delta_{ij}$ hold before quotienting and hence hold on $M$. Its [basis](../../../vector-space.md#basis) consists of the monomials $x^\alpha$ with $0\le\alpha_i<p$, so **$\dim_kM=p^n>0$**. This is the explicit finite-dimensional module for the [Weyl algebra in positive characteristic](../../../noncommutative-algebra.md#weyl-algebra-in-positive-characteristic).

Therefore condition (b) fails in positive characteristic and implies characteristic zero. Combining this with the preceding two implications proves **$(a)\Longleftrightarrow(b)\Longleftrightarrow(c)$**. The same representation also has nonzero proper kernel, since the infinite-dimensional [Weyl algebra](../../../noncommutative-algebra.md#weyl-algebra) cannot inject into a finite-dimensional endomorphism [algebra](../../../algebra.md), confirming its failure of simplicity in positive characteristic.

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

The [Bernstein inequality for Weyl algebra modules](../../../associative-algebra.md#bernstein-inequality-for-weyl-algebra-modules) requires characteristic zero: for a nonzero finitely generated left or right [module](../../../module-theory.md#module-mathematics) $M$ over $A_n(k)$,

$$
\boxed{\operatorname{GKdim}_{A_n(k)}M\ge n.}
$$

Equivalently, its [Bernstein growth dimension of a Weyl algebra module](../../../associative-algebra.md#bernstein-growth-dimension-of-a-weyl-algebra-module) is at least $n$. Without the characteristic-zero hypothesis this is false, as the module in part (c) has dimension zero in the growth sense. The proof below works over any characteristic-zero [field](../../../algebra.md#field), not just an algebraically closed one.

For a left [module](../../../module-theory.md#module-mathematics), choose a nonzero finite-dimensional generating subspace $M_0$ and put $M_j=F_jA_n\,M_0$, where $F_j$ is the [Bernstein filtration](../../../noncommutative-algebra.md#bernstein-filtration). Ordered [monomials](../../../polynomial.md#monomial) give

$$
\dim_kF_jA_n=\binom{j+2n}{2n}.
$$

Multiplication defines the linear action map

$$
F_jA_n\longrightarrow\operatorname{Hom}_k(M_j,M_{2j}),\qquad a\longmapsto(m\mapsto am).
$$

We prove this map injective by induction on $j$, which is the essential [faithful finite-step action of a Weyl algebra](../../../associative-algebra.md#faithful-finite-step-action-of-a-weyl-algebra) argument. For $j=0$, an element is a [scalar](../../../vector-space.md#scalar), and a scalar killing $M_0\ne0$ is zero. Suppose $a\in F_j$ kills $M_j$. For any generator $z$ and $m\in M_{j-1}$, both $azm$ and $zam$ vanish because $zm\in M_j$ and $m\in M_j$. Thus $[a,z]\in F_{j-1}$ kills $M_{j-1}$, so induction gives $[a,z]=0$ for every generator. By the explicit commutator formulas in part (a), commuting with all $D_i$ forces all positive $x_i$ exponents of $a$ to vanish, and commuting with all $x_i$ forces all positive $D_i$ exponents to vanish. Characteristic zero is used to cancel the nonzero integer exponents. Hence $a$ is scalar and, because it kills $M_0$, is zero. This proves injectivity.

Taking dimensions yields

$$
\binom{j+2n}{2n}\le(\dim_kM_j)(\dim_kM_{2j})\le(\dim_kM_{2j})^2.
$$

The left side is asymptotic to $j^{2n}/(2n)!$. Consequently $\dim_kM_{2j}\ge Cj^n$ for all sufficiently large $j$ and some $C>0$. Taking logarithms and the limsup in the definition of [Gelfand–Kirillov dimension of a module](../../../associative-algebra.md#gelfand-kirillov-dimension-of-a-module) proves the claimed lower bound. For a good [Bernstein filtration](../../../noncommutative-algebra.md#bernstein-filtration), the associated graded [module](../../../module-theory.md#module-mathematics) is finite over $k[x_1,\ldots,x_n,\xi_1,\ldots,\xi_n]$; its cumulative Hilbert function is eventually polynomial, and the same comparison says its degree is at least $n$.

For right [modules](../../../module-theory.md#module-mathematics), use the [opposite ring](../../../commutative-algebra.md#opposite-ring) isomorphism $A_n(k)\cong A_n(k)^{\mathrm{op}}$ sending $x_i$ to $x_i$ and $D_i$ to $-D_i$. It respects the [Bernstein filtration](../../../noncommutative-algebra.md#bernstein-filtration), so the identical estimate applies. The bound is sharp: the polynomial [module](../../../module-theory.md#module-mathematics) $k[x_1,\ldots,x_n]$, generated by $1$, has $M_j$ equal to the polynomials of degree at most $j$, of dimension $\binom{j+n}{n}$. Its [Gelfand–Kirillov dimension of a module](../../../associative-algebra.md#gelfand-kirillov-dimension-of-a-module) is exactly $n$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
