# Paper 128

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_128.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_128.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) is $J(A)=\bigcap_L L$, where $L$ runs over the [maximal right ideals](../../../associative-algebra.md#maximal-right-ideal) of $A$; equivalently, it is the intersection of the [annihilators](../../../module-theory.md#annihilator-ring-theory) of all [simple modules](../../../module-theory.md#irreducible-module). It is a two-sided [ideal](../../../commutative-algebra.md#ideal). A [projective module](../../../module-theory.md#projective-module) has the lifting property against every surjective [R-module homomorphism](../../../module-theory.md#module-homomorphism). A [finitely generated module](../../../module-theory.md#finitely-generated-module) is a [projective module](../../../module-theory.md#projective-module) precisely when it is a [direct summand](../../../vector-space.md#direct-summand) of a finitely generated [free module](../../../module-theory.md#free-module). An [indecomposable module](../../../module-theory.md#indecomposable-module) is nonzero and admits no [direct sum](../../../vector-space.md#direct-sum) decomposition into two nonzero [submodules](../../../module-theory.md#submodule).

To calculate the [top of an indecomposable projective module](../../../module-theory.md#top-of-an-indecomposable-projective-module), use the [right Artinian ring](../../../noncommutative-algebra.md#right-artinian-ring) hypothesis, namely the [descending chain condition](../../../algebra.md#descending-chain-condition) on [right ideals](../../../associative-algebra.md#right-ideal). The [Hopkins-Levitzki theorem](../../../noncommutative-algebra.md#hopkins-levitzki-theorem) gives finite [composition length](../../../finite-group-theory.md#composition-length) of the right regular [module](../../../module-theory.md#module-mathematics), hence of its [submodule](../../../module-theory.md#submodule) $P$. Also $J=J(A)$ is a [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal), and $A/J$ is a [semisimple ring](../../../commutative-algebra.md#semisimple-ring). Thus the [quotient module](../../../module-theory.md#quotient-module) $\overline P=P/PJ$ is a [semisimple module](../../../module-theory.md#semisimple-module); it is nonzero, since $P=PJ$ would imply $P=PJ^m=0$ for sufficiently large $m$.

Suppose $\overline P$ were not a [simple module](../../../module-theory.md#irreducible-module). A nontrivial [direct sum](../../../vector-space.md#direct-sum) decomposition of this [semisimple module](../../../module-theory.md#semisimple-module) would give an [idempotent](../../../commutative-algebra.md#idempotent) $\alpha\in\operatorname{End}_A(\overline P)$ that is neither zero nor the identity. Writing $\pi:P\to\overline P$, the lifting property of the [projective module](../../../module-theory.md#projective-module) $P$ gives $\beta\in\operatorname{End}_A(P)$ with $\pi\beta=\alpha\pi$. The [Fitting lemma](../../../module-theory.md#fitting-lemma) for an [indecomposable module](../../../module-theory.md#indecomposable-module) of finite [composition length](../../../finite-group-theory.md#composition-length) says that $\beta$ is either invertible or a [nilpotent element](../../../commutative-algebra.md#nilpotent). Its induced map $\alpha$ would then be invertible or a [nilpotent element](../../../commutative-algebra.md#nilpotent), respectively. Neither is possible for a nontrivial [idempotent](../../../commutative-algebra.md#idempotent). Therefore **$P/PJ(A)$ is simple**. This argument does not assume that an embedded [projective module](../../../module-theory.md#projective-module) automatically splits off from the ambient [module](../../../module-theory.md#module-mathematics).

A [block of an Artinian algebra](../../../associative-algebra.md#block-of-an-artinian-algebra) is a nonzero two-sided [direct summand](../../../vector-space.md#direct-summand) $Ae$ determined by a [primitive central idempotent](../../../associative-algebra.md#primitive-central-idempotent) $e$: $e$ cannot be written as a sum of two nonzero orthogonal [central idempotents](../../../associative-algebra.md#central-idempotent). Its identity is $e$. For a finite-dimensional [associative algebra](../../../associative-algebra.md), the [blocks of an Artinian algebra](../../../associative-algebra.md#block-of-an-artinian-algebra) give its unique decomposition as a finite product of indecomposable [algebras](../../../algebra.md), or equivalently as a [direct sum](../../../vector-space.md#direct-sum) of two-sided [ideals](../../../commutative-algebra.md#ideal).

For the [block of S3 in characteristic three](../../../representation-theory.md#block-of-s3-in-characteristic-three), put $A=kS_3$, $r=(123)$, $s=(12)$ and $a=r-1$. The [group algebra](../../../associative-algebra.md#group-algebra) has [basis](../../../vector-space.md#basis) $r^i,r^is$ for $0\leq i<3$. In [characteristic](../../../algebra.md#characteristic-of-a-field) three,

$$
a^3=0,\qquad sas=r^{-1}-1=-a+a^2.
$$

Consequently $I=aA$ is a two-sided [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal), $I^3=0$, and $A/I\cong kC_2\cong k\times k$. A [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal) lies in the [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical), and a quotient that is a [semisimple ring](../../../commutative-algebra.md#semisimple-ring) forces the reverse inclusion. Hence

$$
\boxed{J(A)=aA,\qquad \dim_k J(A)=4.}
$$

Define orthogonal [idempotents](../../../commutative-algebra.md#idempotent) $e_+=(1+s)/2$ and $e_-=(1-s)/2$. They sum to one, so the right regular [module](../../../module-theory.md#module-mathematics) decomposes as

$$
\boxed{kS_3=e_+A\oplus e_-A,\qquad \dim_k e_+A=\dim_k e_-A=3.}
$$

The two summands are the [indecomposable projectives of S3 in characteristic three](../../../representation-theory.md#indecomposable-projectives-of-s3-in-characteristic-three). Each [direct summand](../../../vector-space.md#direct-summand) is a [projective module](../../../module-theory.md#projective-module), with [basis](../../../vector-space.md#basis) $e_\pm,e_\pm r,e_\pm r^2$. Its [quotient module](../../../module-theory.md#quotient-module) modulo multiplication by $J(A)$ is one-dimensional: the [trivial representation](../../../representation-theory.md#trivial-representation) for $e_+A$, and the [sign representation](../../../representation-theory-of-the-symmetric-group.md#sign-representation) for $e_-A$. Each is an [indecomposable module](../../../module-theory.md#indecomposable-module), since two nonzero [direct summands](../../../vector-space.md#direct-summand) would each have nonzero [quotient module](../../../module-theory.md#quotient-module) modulo $J(A)$, contradicting its one-dimensional top. For additional detail, the successive factors of the [radical series of a module](../../../module-theory.md#radical-series-of-a-module) are the [trivial representation](../../../representation-theory.md#trivial-representation), [sign representation](../../../representation-theory-of-the-symmetric-group.md#sign-representation), [trivial representation](../../../representation-theory.md#trivial-representation) for $e_+A$, and the [sign representation](../../../representation-theory-of-the-symmetric-group.md#sign-representation), [trivial representation](../../../representation-theory.md#trivial-representation), [sign representation](../../../representation-theory-of-the-symmetric-group.md#sign-representation) for $e_-A$. Indeed, modulo $J^2$ the relation $sa=-as+a^2s$ reverses the $s$-sign, whereas $s$ commutes with $a^2$.

The [center of an associative algebra](../../../associative-algebra.md#center-of-an-associative-algebra) is spanned by the [conjugacy class](../../../group-theory.md#conjugacy-class) sums $1$, $r+r^2$, and $(1+r+r^2)s$. Since $r+r^2=-1+a^2$ and $1+r+r^2=a^2$, this [center of an associative algebra](../../../associative-algebra.md#center-of-an-associative-algebra) is

$$
Z(A)=k1\oplus ka^2\oplus ka^2s.
$$

Its [vector subspace](../../../vector-space.md#vector-subspace) $ka^2\oplus ka^2s$ is a [square-zero ideal](../../../commutative-algebra.md#square-zero-ideal). If $d1+n$ is a [central idempotent](../../../associative-algebra.md#central-idempotent), then $d^2=d$ and $(2d-1)n=0$. Thus $d=0$ or $1$ and $n=0$. There is no nontrivial [central idempotent](../../../associative-algebra.md#central-idempotent), so **the whole group algebra is its single block**. The two three-dimensional [projective modules](../../../module-theory.md#projective-module) above are a decomposition of the regular [module](../../../module-theory.md#module-mathematics), not two [blocks of an Artinian algebra](../../../associative-algebra.md#block-of-an-artinian-algebra).

## 2

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring) satisfies the [ascending chain condition](../../../algebra.md#ascending-chain-condition) on [right ideals](../../../associative-algebra.md#right-ideal); equivalently, every [right ideal](../../../associative-algebra.md#right-ideal) is a [finitely generated module](../../../module-theory.md#finitely-generated-module).

Here is a [noncommutative Hilbert basis theorem](../../../noncommutative-algebra.md#noncommutative-hilbert-basis-theorem) proof adapted to the stated hypothesis. Set $F_{-1}=0$ and

$$
F_n=\sum_{i=0}^n Ax^i=\sum_{i=0}^n x^iA.
$$

The equality follows inductively from $A+xA=A+Ax$, by moving one coefficient past one $x$ at a time. These spaces form an exhaustive [filtered algebra](../../../module-theory.md#filtered-algebra) structure on $B$, with $F_nF_m\subseteq F_{n+m}$. This does not assert uniqueness of the displayed expressions or the existence of a coefficient-moving [automorphism](../../../algebra.md#automorphism).

For a [right ideal](../../../associative-algebra.md#right-ideal) $I\subseteq B$, define

$$
L_n=\{a\in A:ax^n\in I+F_{n-1}\}.
$$

Each $L_n$ is a [right ideal](../../../associative-algebra.md#right-ideal) of $A$. In fact, if $a\in L_n$ and $c\in A$, write $cx^n=x^nb+u$ with $b\in A$, $u\in F_{n-1}$; then $acx^n=(ax^n)b+au\in I+F_{n-1}$. Also $L_n\subseteq L_{n+1}$ by right multiplication by $x$. Since $A$ is a [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring), this ascending chain stabilizes at some $L_N$.

Choose finite generators $a_{nj}$ for each $L_n$, $0\leq n\leq N$, and choose $f_{nj}\in I$ with $f_{nj}-a_{nj}x^n\in F_{n-1}$. These finitely many elements generate $I$ as a [right ideal](../../../associative-algebra.md#right-ideal). To see this, induct on $m$ for $f\in I\cap F_m$. Write $f=ax^m+u$ with $u\in F_{m-1}$; then $a\in L_m$. Put $d=\min(m,N)$ and express $a=\sum_j a_{dj}c_j$. Write $c_jx^d=x^db_j+u_j$ with $u_j\in F_{d-1}$. The difference

$$
f-\sum_j f_{dj}b_jx^{m-d}
$$

lies in $I\cap F_{m-1}$, so the induction applies. At $m=0$ the remainder is zero. Hence **$B$ is right Noetherian**.

For the [quantum torus](../../../noncommutative-algebra.md#quantum-torus), take $q\in k^\times$ and the convention $YX=qXY$. Begin with the [polynomial ring](../../../commutative-algebra.md#polynomial-ring) $k[X]$, which is [Noetherian](../../../algebra.md#noetherian-ring) by the [Hilbert basis theorem](../../../algebra.md#hilbert-basis-theorem). Adjoining $X^{-1}$ preserves the hypothesis because it commutes with $k[X]$, and gives $k[X^{\pm1}]$. Adjoin $Y$ next. The relation $Yf(X)=f(qX)Y$ and its inverse coefficient-moving relation give $A+YA=A+AY$ for $A=k[X^{\pm1}]$. Finally adjoin $Y^{-1}$ to $k[X^{\pm1}][Y;\sigma]$, where $\sigma(X)=qX$. On a [monomial](../../../polynomial.md#monomial), $Y^{-1}X^iY^j=q^{-i}X^iY^{j-1}$; when $j=0$ this is in $AY^{-1}$, and when $j>0$ it is in $A$. The reverse inclusion follows by the same relation. The preceding argument applies at each step, proving **the quantum torus is right Noetherian**. Nonzero $q$ is required for this notation.

For a [noncommutative ring](../../../commutative-algebra.md#noncommutative-ring), a [prime ideal of a noncommutative ring](../../../noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring) means a proper two-sided [ideal](../../../commutative-algebra.md#ideal) $P$ such that $UV\subseteq P$ for two-sided [ideals](../../../commutative-algebra.md#ideal) $U,V$ implies $U\subseteq P$ or $V\subseteq P$. Equivalently, $aAb\subseteq P$ implies $a\in P$ or $b\in P$. This definition does not require $A/P$ to be a [noncommutative domain](../../../noncommutative-algebra.md#noncommutative-domain).

Retain the [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring) hypothesis for the last assertion. More generally, the [ascending chain condition](../../../algebra.md#ascending-chain-condition) on two-sided [ideals](../../../commutative-algebra.md#ideal) suffices. We claim that every proper two-sided [ideal](../../../commutative-algebra.md#ideal) $I$ contains a product of finitely many [prime ideals of a noncommutative ring](../../../noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring), each containing $I$. If not, choose a maximal counterexample $I$. It cannot be a [prime ideal of a noncommutative ring](../../../noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring). Thus there are two-sided [ideals](../../../commutative-algebra.md#ideal) $U,V$ strictly containing $I$ with $UV\subseteq I$: add $I$ to the two witnesses for failure of the defining condition for a [prime ideal of a noncommutative ring](../../../noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring). By maximality, both $U$ and $V$ contain products of finitely many [prime ideals of a noncommutative ring](../../../noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring) containing them. Concatenating these products gives a product inside $UV\subseteq I$, a contradiction.

Apply the claim to $I=0$ in a nonzero $A$, obtaining $P_1\cdots P_r=0$. Every [prime ideal of a noncommutative ring](../../../noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring) $Q$ contains one of the $P_i$, by repeated application of the definition of a [prime ideal of a noncommutative ring](../../../noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring). For the [prime radical of a noncommutative ring](../../../noncommutative-algebra.md#prime-radical-of-a-noncommutative-ring) $N$, it follows that

$$
\boxed{N=P_1\cap\cdots\cap P_r,\qquad N^r=0.}
$$

Indeed, $N\subseteq P_i$ gives $N^r\subseteq P_1\cdots P_r=0$, and $\bigcap_iP_i\subseteq Q$ for every $Q$ gives equality of the intersections. If $A=0$, the empty intersection is the whole zero [ring](../../../commutative-algebra.md#ring) and the conclusion is immediate.

The final assertion is false for arbitrary [algebras](../../../algebra.md) without the preceding chain condition. For example, in the commutative [ring](../../../commutative-algebra.md#ring) $k[z_1,z_2,\ldots]/(z_i^2:i\geq1)$ the [nilradical](../../../commutative-algebra.md#nilradical) is $(z_1,z_2,\ldots)$, its only [prime ideal](../../../commutative-algebra.md#prime-ideal), but the product of any number of distinct $z_i$ is nonzero. Thus this [nilradical](../../../commutative-algebra.md#nilradical) is not a [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal).

## 3

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use $q\in k^\times$ and $YX=qXY$ for the [quantum plane](../../../noncommutative-algebra.md#quantum-plane). Its [monomials](../../../polynomial.md#monomial) $X^iY^j$, $i,j\geq0$, form a [basis](../../../vector-space.md#basis), with multiplication

$$
(X^iY^j)(X^uY^v)=q^{ju}X^{i+u}Y^{j+v}.
$$

One way to verify the [basis](../../../vector-space.md#basis) assertion without assuming it is to define this multiplication on the [vector space](../../../vector-space.md) with the displayed formal [basis](../../../vector-space.md#basis). This defines an [associative algebra](../../../associative-algebra.md): for a third [monomial](../../../polynomial.md#monomial) $X^wY^z$, the two products of three [monomials](../../../polynomial.md#monomial) have the same exponent $ju+jw+vw$ of $q$, and its generators satisfy the required relation. Conversely, the relation puts every word into this form, establishing the presentation. Order exponent pairs by the [lexicographic order](../../../extremal-set-theory.md#lexicographic-order). The largest [monomials](../../../polynomial.md#monomial) of two nonzero finite sums give the uniquely largest [monomial](../../../polynomial.md#monomial) of their product, with coefficient $c d q^{ju}\ne0$. Therefore **the quantum plane is a domain**. If one allows $q=0$, the assertion fails because $YX=0$ with both factors nonzero.

A [uniform module](../../../module-theory.md#uniform-module) is a nonzero [module](../../../module-theory.md#module-mathematics) in which any two nonzero [submodules](../../../module-theory.md#submodule) have nonzero intersection. Suppose the right regular [module](../../../module-theory.md#module-mathematics) of a [right Noetherian domain](../../../noncommutative-algebra.md#right-noetherian-domain) $A$ were not a [uniform module](../../../module-theory.md#uniform-module). Choose nonzero $a,b$ from two [right ideals](../../../associative-algebra.md#right-ideal) with zero intersection. Then $aA\cap bA=0$. The [right ideals](../../../associative-algebra.md#right-ideal)

$$
aA,\ baA,\ b^2aA,\ldots
$$

form a [direct sum](../../../vector-space.md#direct-sum). For if $\sum_{i=0}^m b^ia c_i=0$, then $ac_0\in aA\cap bA$ is zero, so $c_0=0$ by the [noncommutative domain](../../../noncommutative-algebra.md#noncommutative-domain) property. Cancel the nonzero factor $b$ on the left and repeat to obtain every $c_i=0$. Each summand is nonzero, so their finite partial sums form a strictly ascending chain of [right ideals](../../../associative-algebra.md#right-ideal). This contradicts the [ascending chain condition](../../../algebra.md#ascending-chain-condition) of a [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring). Hence **$A$ is a uniform right module**.

It follows that $aA\cap sA\ne0$ whenever $a,s\ne0$: there are nonzero $u,v$ with $au=sv$. This is the [right Ore condition](../../../noncommutative-algebra.md#right-ore-condition) for the multiplicative set $S=A\setminus\{0\}$; zero numerators cause no difficulty. The [Ore localization](../../../noncommutative-algebra.md#ore-localization) theorem therefore constructs the [ring](../../../commutative-algebra.md#ring) of right fractions

$$
\boxed{Q=AS^{-1}=\{as^{-1}:a\in A,\ s\ne0\},\qquad A\hookrightarrow Q.}
$$

The map is injective because an element mapping to zero is annihilated on the right by some nonzero denominator, impossible in a [noncommutative domain](../../../noncommutative-algebra.md#noncommutative-domain). To make the denominator convention concrete, if $su=tv\ne0$ then

$$
as^{-1}+bt^{-1}=(au+bv)(su)^{-1}.
$$

For multiplication, choose $bu=sc$ with $u\ne0$; then

$$
(as^{-1})(bt^{-1})=ac(tu)^{-1}.
$$

Common right multiples make these operations independent of the chosen representatives. Every nonzero $as^{-1}$ has inverse $sa^{-1}$, so $Q$ is a [division ring](../../../commutative-algebra.md#division-ring). The original [field](../../../algebra.md#field) $k$ is central in $A$ and therefore in the inverses as well, making $Q$ a [division algebra](../../../algebra.md#division-algebra) over $k$. No commutative [fraction field](../../../commutative-algebra.md#field-of-fractions) construction is being assumed.

## 4

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Choose a finite-dimensional generating [vector subspace](../../../vector-space.md#vector-subspace) $V\subseteq A$ containing $1$, and write $V^n$ for the [linear span](../../../vector-space.md#linear-span) of products of $n$ elements of $V$. The [Gelfand–Kirillov dimension](../../../associative-algebra.md#gelfand-kirillov-dimension) is

$$
\boxed{\operatorname{GKdim}A=\limsup_{n\to\infty}\frac{\log\dim_k V^n}{\log n}.}
$$

For a nonzero [finitely generated module](../../../module-theory.md#finitely-generated-module) $M$ considered as a right [module](../../../module-theory.md#module-mathematics), choose a finite-dimensional generating [vector subspace](../../../vector-space.md#vector-subspace) $W\subseteq M$ and define the [Gelfand–Kirillov dimension of a module](../../../associative-algebra.md#gelfand-kirillov-dimension-of-a-module) by

$$
\boxed{\operatorname{GKdim}_A M=\limsup_{n\to\infty}\frac{\log\dim_k(WV^n)}{\log n}.}
$$

For left [modules](../../../module-theory.md#module-mathematics), replace $WV^n$ by $V^nW$. These values are independent of the choices: two algebra-generating [vector subspaces](../../../vector-space.md#vector-subspace) satisfy $V\subseteq (V')^c$ and $V'\subseteq V^d$ for some positive integers $c,d$, and two module-generating [vector subspaces](../../../vector-space.md#vector-subspace) are contained in bounded-degree translates of one another. The corresponding growth bounds differ only by a constant rescaling and shift of $n$, which do not change the [limit superior](../../../real-analysis.md#limit-superior).

Let $S$ be a nonzero [standard graded algebra](../../../commutative-algebra.md#standard-graded-algebra), generated by $r$ elements of degree one. It is a homogeneous [quotient ring](../../../commutative-algebra.md#quotient-ring) of the [polynomial ring](../../../commutative-algebra.md#polynomial-ring) $k[z_1,\ldots,z_r]$. By the [Hilbert-Serre theorem](../../../commutative-algebra.md#hilbert-serre-theorem), its [Hilbert series](../../../commutative-algebra.md#hilbert-series) is a rational function whose only possible pole is at $t=1$. After canceling, write it as $P(t)/(1-t)^d$ with $P(1)\ne0$, where $0\leq d\leq r$. The cumulative dimensions are the coefficients of $P(t)/(1-t)^{d+1}$ and are eventually a [polynomial](../../../polynomial.md) in $n$ of degree $d$, with positive leading coefficient. With $V=S_0\oplus S_1$, these cumulative dimensions equal $\dim V^n$. Consequently

$$
\boxed{\operatorname{GKdim}S=d\in\{0,1,\ldots,r\}.}
$$

For $d=0$ the [algebra](../../../algebra.md) is finite-dimensional and nonzero, so the cumulative dimension is eventually a positive constant. If the zero [algebra](../../../algebra.md) is allowed, the common convention $\operatorname{GKdim}0=-\infty$ is an exception to the printed assertion; the integer conclusion concerns nonzero unital [algebras](../../../algebra.md).

For the [Weyl algebra](../../../noncommutative-algebra.md#weyl-algebra) $A=A_1(k)=k\langle X,D\rangle/(DX-XD-1)$, the total-degree [filtered algebra](../../../module-theory.md#filtered-algebra) structure has [associated graded ring](../../../commutative-algebra.md#associated-graded-ring) $\operatorname{gr}A=k[x,\xi]$. Its ordered [monomials](../../../polynomial.md#monomial) $X^iD^j$ form a [basis](../../../vector-space.md#basis). Every [finitely generated module](../../../module-theory.md#finitely-generated-module) has a [good filtration of a module](../../../module-theory.md#good-filtration-of-a-module), and its [associated graded module](../../../commutative-algebra.md#associated-graded-module) is finitely generated over $k[x,\xi]$. The [Hilbert-Serre theorem](../../../commutative-algebra.md#hilbert-serre-theorem) therefore shows that its [Gelfand–Kirillov dimension](../../../associative-algebra.md#gelfand-kirillov-dimension) is an integer in $\{0,1,2\}$.

A nonzero [module](../../../module-theory.md#module-mathematics) of [Gelfand–Kirillov dimension](../../../associative-algebra.md#gelfand-kirillov-dimension) zero here would have eventually constant cumulative dimension, hence be finite-dimensional. This is impossible in [characteristic](../../../algebra.md#characteristic-of-a-field) zero: taking the [trace](../../../linear-algebra.md#matrix-trace) of the [endomorphisms](../../../algebra.md#endomorphism) representing $DX-XD=1$ gives $0=\dim_k M$. For right [modules](../../../module-theory.md#module-mathematics) the right-action operators reverse composition and give the negative identity instead, with the same contradiction. Thus

$$
\boxed{\operatorname{GKdim}_A M\in\{1,2\}.}
$$

Both occur. The regular [module](../../../module-theory.md#module-mathematics) $A$ has $\dim V^n=\binom{n+2}{2}$, hence [Gelfand–Kirillov dimension](../../../associative-algebra.md#gelfand-kirillov-dimension) two. For a right [module](../../../module-theory.md#module-mathematics) of [Gelfand–Kirillov dimension](../../../associative-algebra.md#gelfand-kirillov-dimension) one, take $M=k[x]$ with $f\cdot X=xf$ and $f\cdot D=-f'$. These actions satisfy the defining relation because $(f\cdot D)\cdot X-(f\cdot X)\cdot D=f$. The [module](../../../module-theory.md#module-mathematics) is a [cyclic module](../../../module-theory.md#cyclic-module) generated by $1$, and $\dim(1\cdot V^n)=n+1$. This also gives the lower bound for this particular [Weyl algebra](../../../noncommutative-algebra.md#weyl-algebra) without invoking a general inequality for higher [Weyl algebras](../../../noncommutative-algebra.md#weyl-algebra).

## 5

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Put $A^e=A\otimes_k A^{\mathrm{op}}$, so an $A$-[bimodule](../../../module-theory.md#bimodule) is a left $A^e$-[module](../../../module-theory.md#module-mathematics) through $(a\otimes b^{\mathrm{op}})m=amb$. The [Hochschild cohomology](../../../associative-algebra.md#hochschild-cohomology) is

$$
\boxed{HH^n(A,M)=\operatorname{Ext}_{A^e}^n(A,M).}
$$

Equivalently, the [Hochschild cochain complex](../../../associative-algebra.md#hochschild-cochain-complex) has $C^n(A,M)=\operatorname{Hom}_k(A^{\otimes n},M)$ and [coboundary map](../../../algebra.md#coboundary-map)

$$
(\delta f)(a_1,\ldots,a_{n+1})=a_1f(a_2,\ldots,a_{n+1})+\sum_{i=1}^n(-1)^if(a_1,\ldots,a_ia_{i+1},\ldots,a_{n+1})+(-1)^{n+1}f(a_1,\ldots,a_n)a_{n+1}.
$$

Its [cohomology](../../../cohomology.md) agrees with the displayed [Ext functor](../../../algebra.md#ext-functor) because the [bar resolution of an associative algebra](../../../algebra.md#bar-resolution-of-an-associative-algebra) is free over $A^e$ when $k$ is a [field](../../../algebra.md#field). The [Hochschild cohomological dimension](../../../associative-algebra.md#hochschild-cohomological-dimension) is

$$
\boxed{\operatorname{Dim}(A)=\operatorname{pd}_{A^e}A=\sup\{n:HH^n(A,N)\ne0\text{ for some bimodule }N\}.}
$$

The supremum uses all [bimodules](../../../module-theory.md#bimodule), not merely the finitely generated one supplied in the question; an unbounded [projective dimension](../../../module-theory.md#projective-dimension) is infinity.

An extension in this classification is a [square-zero extension of an algebra](../../../commutative-algebra.md#square-zero-extension-of-an-algebra): a short [exact sequence](../../../homology.md#exact-sequence) $0\to M\to E\to A\to0$, where $E$ and $A$ are unital [algebras](../../../algebra.md), $E\to A$ is unital, and $M$ is its two-sided [ideal](../../../commutative-algebra.md#ideal) with $M^2=0$ and induced $A$-[bimodule](../../../module-theory.md#bimodule) structure equal to the prescribed one. An equivalence of extensions is an [algebra isomorphism](../../../algebra.md#algebra-isomorphism) of the middle terms commuting with the maps and inducing the identity on both $A$ and $M$. Arbitrary isomorphisms of middle [algebras](../../../algebra.md), or extensions without the [square-zero ideal](../../../commutative-algebra.md#square-zero-ideal) requirement, are not classified by this [cohomology](../../../cohomology.md) group.

Choose a $k$-[linear map](../../../vector-space.md#linear-map) section $s:A\to E$ with $s(1)=1$. Its multiplication defect

$$
\mu(a,b)=s(a)s(b)-s(ab)\in M
$$

is a normalized [Hochschild cocycle](../../../associative-algebra.md#hochschild-cocycle): $\mu(1,a)=\mu(a,1)=0$, and [associativity](../../../group.md#associative-property) in $E$ gives $\delta\mu=0$. Changing $s$ to $s+g$, where $g(1)=0$, changes the defect to $\mu+\delta g$, since $M^2=0$.

Conversely, for a normalized [Hochschild cocycle](../../../associative-algebra.md#hochschild-cocycle) $\mu$, put $E_\mu=A\oplus M$ as a [vector space](../../../vector-space.md) and define

$$
(a,m)(b,n)=(ab,an+mb+\mu(a,b)).
$$

The [Hochschild cocycle](../../../associative-algebra.md#hochschild-cocycle) equation is exactly [associativity](../../../group.md#associative-property), and $(1,0)$ is the identity. If $\mu'=\mu+\delta g$, the map $E_{\mu'}\to E_\mu$, $(a,m)\mapsto(a,m+g(a))$, is an equivalence. Conversely, every equivalence has this form after choosing sections. The [normalized Hochschild cochain complex](../../../associative-algebra.md#normalized-hochschild-cochain-complex) computes the same [cohomology](../../../cohomology.md) as the full complex: in the [bar resolution of an associative algebra](../../../algebra.md#bar-resolution-of-an-associative-algebra), the degenerate terms containing an inserted identity form a contractible subcomplex. Passing to the normalized [bar resolution of an associative algebra](../../../algebra.md#bar-resolution-of-an-associative-algebra), then applying the [Hom functor](../../../algebra.md#hom-functor), gives the same [cohomology](../../../cohomology.md). Thus every class has a normalized representative. We obtain **a bijection between $HH^2(A,M)$ and equivalence classes of square-zero extensions**.

For a [formal associative deformation](../../../associative-algebra.md#formal-associative-deformation), a completion convention is necessary. The usual [star product](../../../associative-algebra.md#formal-associative-deformation) lives on the [formal power series module](../../../commutative-algebra.md#formal-power-series-module)

$$
A[[t]]=\varprojlim_r A\otimes_k k[t]/(t^r).
$$

This is the [adic completion of a module](../../../commutative-algebra.md#adic-completion-of-a-module) applied to the ordinary [tensor product](../../../linear-algebra.md#tensor-product), rather than literally the ordinary $A\otimes_k k[[t]]$ when $A$ is infinite-dimensional. For example, $\sum_{n\geq0}X^nt^n$ lies in $k[X][[t]]$ but not in the ordinary [tensor product](../../../linear-algebra.md#tensor-product), whose coefficient spaces have finite-dimensional span. The two agree when $A$ is finite-dimensional. We interpret the printed notation in this standard completed sense; the infinite iteration below requires that interpretation.

A [star product](../../../associative-algebra.md#formal-associative-deformation) is a $k[[t]]$-bilinear, unital product continuous for the [adic topology](../../../commutative-algebra.md#adic-topology) satisfying [associativity](../../../group.md#associative-property) of the form

$$
a*b=ab+\sum_{r\geq1}t^r\mu_r(a,b),\qquad \mu_r\in\operatorname{Hom}_k(A\otimes A,A),\quad \mu_r(1,a)=\mu_r(a,1)=0.
$$

It is a [trivial formal deformation](../../../associative-algebra.md#trivial-formal-deformation) if a $k[[t]]$-linear [automorphism](../../../algebra.md#automorphism) continuous for the [adic topology](../../../commutative-algebra.md#adic-topology) $T=\operatorname{id}+\sum_{r\geq1}t^rT_r$, with $T(1)=1$, satisfies $T(a*b)=T(a)T(b)$.

If $\operatorname{Dim}(A)\leq1$, then $HH^2(A,A)=0$. Suppose changes of coordinates have removed all coefficients below order $r$. The order-$r$ part of [associativity](../../../group.md#associative-property) then says $\delta\mu_r=0$. Hence $\mu_r=\delta g_r$ for a $k$-linear map $g_r:A\to A$. Its normalization gives $g_r(1)=0$, since $(\delta g_r)(1,1)=g_r(1)$. Transport the product by $T_r=\operatorname{id}+t^rg_r$:

$$
a*'b=T_r\bigl(T_r^{-1}(a)*T_r^{-1}(b)\bigr).
$$

The order-$r$ coefficient becomes $\mu_r-\delta g_r=0$, and lower coefficients remain zero. Repeating constructs compatible changes of coordinates modulo every $t^N$. They converge in the [adic topology](../../../commutative-algebra.md#adic-topology) to an invertible $T$ fixing $1$, with inverse obtained coefficient by coefficient. The limit product is ordinary multiplication. Therefore **every star product is trivial under the completed formal-series convention**. In fact, the argument only needs the vanishing of $HH^2(A,A)$, not all of [Hochschild cohomological dimension](../../../associative-algebra.md#hochschild-cohomological-dimension) at most one.

## 6

↑ **Parent:** [Paper 128](paper-128.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [derivation of an algebra](../../../associative-algebra.md#derivation-of-an-algebra) is a $k$-linear map $D:A\to A$ satisfying $D(ab)=D(a)b+aD(b)$. The [commutator](../../../lie-algebra.md#commutator) $[D,E]=D\circ E-E\circ D$ is again a [derivation](../../../associative-algebra.md#derivation-of-an-algebra): expanding $[D,E](ab)$ cancels the two mixed terms and leaves $[D,E](a)b+a[D,E](b)$. The [commutator](../../../lie-algebra.md#commutator) on [endomorphisms](../../../algebra.md#endomorphism) is bilinear, antisymmetric, and satisfies the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) by cancellation of its twelve triple-composition terms. Therefore **$\operatorname{Der}_k(A)$ is a [Lie algebra](../../../lie-algebra.md)**.

In degree zero of the [Hochschild cochain complex](../../../associative-algebra.md#hochschild-cochain-complex), $\delta a(b)=ba-ab$, so $HH^0(A,A)=Z(A)=A$ for commutative $A$. In degree one, $\delta D=0$ is precisely the [derivation](../../../associative-algebra.md#derivation-of-an-algebra) rule; the boundaries are [inner derivations](../../../associative-algebra.md#inner-derivation), which vanish for commutative $A$. Hence

$$
\boxed{HH^0(A,A)=A,\qquad HH^1(A,A)=\operatorname{Der}_k(A).}
$$

For cochains $f\in C^p(A,A)$, $g\in C^q(A,A)$, the [Hochschild cup product](../../../associative-algebra.md#hochschild-cup-product) is

$$
(f\smile g)(a_1,\ldots,a_{p+q})=f(a_1,\ldots,a_p)g(a_{p+1},\ldots,a_{p+q}).
$$

Define the insertion operation by

$$
f\circ g=\sum_{i=0}^{p-1}(-1)^{i(q-1)}f(a_1,\ldots,a_i,g(a_{i+1},\ldots,a_{i+q}),a_{i+q+1},\ldots,a_{p+q-1}).
$$

A degree-zero cochain is an element of $A$, inserted with no arguments; for $p=0$ the sum is empty. For the [Gerstenhaber bracket](../../../associative-algebra.md#gerstenhaber-bracket) we use the left [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule) convention, compatible with the unsigned [Hochschild cup product](../../../associative-algebra.md#hochschild-cup-product) just displayed:

$$
\boxed{[f,g]=(-1)^{(p-1)(q-1)}f\circ g-g\circ f.}
$$

Both degree-zero inputs have bracket zero. Another common insertion convention writes $f\circ g-(-1)^{(p-1)(q-1)}g\circ f$; the two brackets differ by $(-1)^{(p-1)(q-1)}$. With an unsigned [Hochschild cup product](../../../associative-algebra.md#hochschild-cup-product), that convention uses the corresponding right [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule). The distinction matters for a degree-two cochain bracketed with a function. Either consistent convention gives the same degree-one [Lie bracket](../../../lie-algebra.md#lie-bracket) and the same [derivation](../../../associative-algebra.md#derivation-of-an-algebra) action on functions.

If $m(a,b)=ab$, this convention gives $\delta f=[m,f]$. The shifted [Jacobi identity](../../../lie-algebra.md#jacobi-identity) and $[m,m]=0$ therefore show that the [Gerstenhaber bracket](../../../associative-algebra.md#gerstenhaber-bracket) respects [Hochschild cocycles](../../../associative-algebra.md#hochschild-cocycle) and the images of the [coboundary map](../../../algebra.md#coboundary-map). The [Hochschild cup product](../../../associative-algebra.md#hochschild-cup-product) and [Gerstenhaber bracket](../../../associative-algebra.md#gerstenhaber-bracket) induce operations on [Hochschild cohomology](../../../associative-algebra.md#hochschild-cohomology). A [Gerstenhaber algebra](../../../commutative-algebra.md#gerstenhaber-algebra) is a [graded algebra](../../../commutative-algebra.md#graded-algebra) $H$ with an associative degree-zero product with the [graded commutative algebra](../../../commutative-algebra.md#graded-commutative-algebra) rule $uv=(-1)^{pq}vu$, and a degree-minus-one [graded Lie bracket](../../../lie-algebra.md#graded-lie-bracket) making the shifted degrees $|u|-1$ into a [graded Lie algebra](../../../lie-algebra.md#graded-lie-algebra). In particular,

$$
[u,v]=-(-1)^{(p-1)(q-1)}[v,u],\qquad
[u,vw]=[u,v]w+(-1)^{(p-1)q}v[u,w]
$$

for [homogeneous elements of a graded algebra](../../../commutative-algebra.md#homogeneous-element-of-a-graded-algebra) of degrees $p,q$. The shifted [Jacobi identity](../../../lie-algebra.md#jacobi-identity) is

$$
[u,[v,w]]=[[u,v],w]+(-1)^{(p-1)(q-1)}[v,[u,w]].
$$

The [Hochschild cup product](../../../associative-algebra.md#hochschild-cup-product) does not make the cochains a [graded commutative algebra](../../../commutative-algebra.md#graded-commutative-algebra) in general, but does make their [cohomology](../../../cohomology.md) a [graded commutative algebra](../../../commutative-algebra.md#graded-commutative-algebra); the insertion operation supplies the homotopy for this assertion and for the [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule). Thus these axioms describe the induced [Gerstenhaber algebra](../../../commutative-algebra.md#gerstenhaber-algebra), not a claim of a [graded commutative algebra](../../../commutative-algebra.md#graded-commutative-algebra) structure on the cochain multiplication itself.

For $A=k[X]$, the enveloping [algebra](../../../algebra.md) is $A^e=k[X_\ell,X_r]$, and

$$
0\longrightarrow A^e\xrightarrow{\ X_\ell-X_r\ }A^e\longrightarrow A\longrightarrow0
$$

is a [projective resolution](../../../algebra.md#projective-resolution). The first map is injective since $A^e$ is an [integral domain](../../../commutative-algebra.md#integral-domain), and its [cokernel](../../../linear-algebra.md#cokernel) is $A$. Applying $\operatorname{Hom}_{A^e}(-,A)$ gives a zero [coboundary map](../../../algebra.md#coboundary-map). Consequently

$$
\boxed{HH^*(k[X],k[X])=k[X]\otimes_k\Lambda(\partial_X),\qquad |\partial_X|=1.}
$$

The [Hochschild cup product](../../../associative-algebra.md#hochschild-cup-product) is ordinary multiplication of functions and scalar multiplication of [derivations](../../../associative-algebra.md#derivation-of-an-algebra), with the product of two [derivations](../../../associative-algebra.md#derivation-of-an-algebra) zero because $HH^2=0$. Every [derivation](../../../associative-algebra.md#derivation-of-an-algebra) is $f\partial_X$, since it is determined by its value on $X$. The [Gerstenhaber bracket](../../../associative-algebra.md#gerstenhaber-bracket) is

$$
[f\partial_X,g\partial_X]=(fg'-gf')\partial_X,\qquad [f\partial_X,h]=fh',\qquad [h_1,h_2]=0,
$$

with all other orders fixed by graded antisymmetry. These formulas fully determine the [Gerstenhaber algebra](../../../commutative-algebra.md#gerstenhaber-algebra).

For $A=k[X,Y]$, the [Hochschild-Kostant-Rosenberg theorem](../../../associative-algebra.md#hochschild-kostant-rosenberg-theorem) identifies

$$
\boxed{HH^*(A,A)=\bigwedge_A^*\operatorname{Der}_k(A)=A\otimes_k\Lambda(\partial_X,\partial_Y).}
$$

Thus the degrees zero, one, and two are $A$, $A\partial_X\oplus A\partial_Y$, and $A(\partial_X\wedge\partial_Y)$, and all higher groups vanish. The [Hochschild-Kostant-Rosenberg](../../../associative-algebra.md#hochschild-kostant-rosenberg-theorem) map sends a wedge of $p$ [derivations](../../../associative-algebra.md#derivation-of-an-algebra) to the cochain

$$
\frac1{p!}\sum_{\sigma\in S_p}\operatorname{sgn}(\sigma)\prod_{j=1}^p D_{\sigma(j)}(a_j).
$$

The factorial is invertible in [characteristic](../../../algebra.md#characteristic-of-a-field) zero. Equivalently, the groups follow from the [Koszul resolution](../../../algebra.md#koszul-resolution) on the [regular sequence](../../../commutative-algebra.md#regular-sequence) $X_\ell-X_r,Y_\ell-Y_r$ in $A^e$, whose dual [coboundary maps](../../../algebra.md#coboundary-map) vanish on $A$.

The [Hochschild cup product](../../../associative-algebra.md#hochschild-cup-product) becomes the [exterior product](../../../linear-algebra.md#exterior-product), and our [Gerstenhaber bracket](../../../associative-algebra.md#gerstenhaber-bracket) becomes the left [Schouten-Nijenhuis bracket](../../../linear-algebra.md#schouten-nijenhuis-bracket). It is determined by the [commutator](../../../lie-algebra.md#commutator) of [derivations](../../../associative-algebra.md#derivation-of-an-algebra), $[D,f]=D(f)$, zero brackets of functions, and the displayed graded antisymmetry and left [graded Leibniz rule](../../../commutative-algebra.md#graded-leibniz-rule). For explicit signs, put $\Pi=\partial_X\wedge\partial_Y$ and $D=F\partial_X+G\partial_Y$. Then

$$
[h\Pi,f]=h(f_Y\partial_X-f_X\partial_Y),\qquad [D,h\Pi]=(D(h)-h(F_X+G_Y))\Pi,\qquad [h\Pi,j\Pi]=0.
$$

The last bracket has degree three, whose [exterior power](../../../linear-algebra.md#exterior-power) is zero. For two [derivations](../../../associative-algebra.md#derivation-of-an-algebra), the coefficient functions of their [commutator](../../../lie-algebra.md#commutator) give the remaining formula. This specifies the entire [Gerstenhaber algebra](../../../commutative-algebra.md#gerstenhaber-algebra); under the alternate insertion convention mentioned above, the first displayed bracket changes sign, together with the Leibniz convention. No smoothness of a general finitely generated commutative [algebra](../../../algebra.md) was assumed: the [Hochschild-Kostant-Rosenberg theorem](../../../associative-algebra.md#hochschild-kostant-rosenberg-theorem) is invoked here only for the smooth [polynomial ring](../../../commutative-algebra.md#polynomial-ring) $k[X,Y]$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
