# Paper 2

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper2.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper2.pdf)

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

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Suppose first that $M$ is a [Noetherian module](../../../algebra.md#noetherian-module). An ascending chain of [submodules](../../../module-theory.md#submodule) of $N$ is also a chain in $M$, so it stabilizes. A chain in the [quotient module](../../../module-theory.md#quotient-module) $M/N$ lifts to a chain in $M$, so it also stabilizes. Thus both $N$ and $M/N$ are [Noetherian modules](../../../algebra.md#noetherian-module).

Conversely, let $M_1\subseteq M_2\subseteq\cdots$ be a chain of [submodules](../../../module-theory.md#submodule) of $M$. If $N$ and $M/N$ are [Noetherian modules](../../../algebra.md#noetherian-module), both $M_i\cap N$ and $(M_i+N)/N$ stabilize, say for $i\geq i_0$. For $x\in M_{i+1}$, equality of the images gives $y\in M_i$ with $x-y\in N$. Then $x-y\in M_{i+1}\cap N=M_i\cap N$, and hence $x\in M_i$. This proves the extension direction of [Noetherian modules in a short exact sequence](../../../algebra.md#noetherian-modules-in-a-short-exact-sequence).

The left regular [module](../../../module-theory.md#module-mathematics) $R$ is [Noetherian](../../../algebra.md#noetherian-ring) because $R$ is a [left Noetherian ring](../../../noncommutative-algebra.md#left-noetherian-ring). Applying the extension result inductively makes each finite [direct sum](../../../vector-space.md#direct-sum) $R^s$ [Noetherian](../../../algebra.md#noetherian-ring). Every [finitely generated module](../../../module-theory.md#finitely-generated-module) on the left is a [quotient module](../../../module-theory.md#quotient-module) of such a [direct sum](../../../vector-space.md#direct-sum), so it is [Noetherian](../../../algebra.md#noetherian-ring).

A [poly-(cyclic or finite) group](../../../group.md#poly-cyclic-or-finite-group) has a finite [subnormal series](../../../group-theory.md#subnormal-series)

$$
1=G_0\triangleleft G_1\triangleleft\cdots\triangleleft G_\ell=G
$$

whose factors are [cyclic groups](../../../group.md#cyclic-group) or [finite groups](../../../group.md#finite-group). We prove that the [group ring](../../../commutative-algebra.md#group-ring) $R[G_i]$ is a [left Noetherian ring](../../../noncommutative-algebra.md#left-noetherian-ring) by induction. Put $A=R[G_{i-1}]$. A finite factor makes $R[G_i]$ a finite free left $A$-[module](../../../module-theory.md#module-mathematics), using a coset transversal. Its [left ideals](../../../associative-algebra.md#left-ideal) are $A$-[submodules](../../../module-theory.md#submodule), so [finite-module extension preserves Noetherianity](../../../noncommutative-algebra.md#finite-module-extension-preserves-noetherianity) handles this case.

If the factor is infinite cyclic, choose a lift $t$ of a generator and let $\sigma(a)=tat^{-1}$. The [group ring](../../../commutative-algebra.md#group-ring) is the [skew Laurent polynomial ring](../../../commutative-algebra.md#skew-laurent-polynomial-ring) $A[t,t^{-1};\sigma]$. Here is the required left-sided [skew Hilbert basis theorem](../../../noncommutative-algebra.md#skew-hilbert-basis-theorem). For a [left ideal](../../../associative-algebra.md#left-ideal) $L\subseteq A[t;\sigma]$, define

$$
I_n=\left\{\sigma^{-n}(a_n):\sum_{j=0}^n a_jt^j\in L\right\}.
$$

Each $I_n$ is a [left ideal](../../../associative-algebra.md#left-ideal) of $A$. Left multiplication by $t$ gives $I_n\subseteq I_{n+1}$. The [ascending chain condition](../../../algebra.md#ascending-chain-condition) makes these ideals constant for $n\geq n_0$; choose finitely many generators for each $I_n$, $0\leq n\leq n_0$, and lift them to polynomials $f_{nj}\in L$.

If $f\in L$ has degree $d\geq n_0$ and leading coefficient $a_d$, write

$$
\sigma^{-d}(a_d)=\sum_j r_j\sigma^{-n_0}(a_{n_0j}).
$$

Subtracting $\sum_j\sigma^d(r_j)t^{d-n_0}f_{n_0j}$ cancels the leading coefficient. For $d<n_0$, use the lifts for $I_d$ instead. Induction on [polynomial degree](../../../polynomial.md#degree-of-a-polynomial) shows that the finitely many $f_{nj}$ generate $L$. Thus the [skew polynomial ring of an automorphism](../../../commutative-algebra.md#skew-polynomial-ring-of-an-automorphism) is a [left Noetherian ring](../../../noncommutative-algebra.md#left-noetherian-ring).

Finally, for a [left ideal](../../../associative-algebra.md#left-ideal) $K$ of $A[t,t^{-1};\sigma]$, its intersection with $A[t;\sigma]$ has finitely many generators. Every $f\in K$ satisfies $t^mf\in A[t;\sigma]$ for some $m\geq0$, so those same generators generate $K$ after multiplication by $t^{-m}$. This completes the induction and proves that **$R[G]$ is left Noetherian**, the left-sided form of [group rings of poly-(cyclic or finite) groups are Noetherian](../../../commutative-algebra.md#group-rings-of-poly-cyclic-or-finite-groups-are-noetherian).

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Jacobson radical](../../../noncommutative-algebra.md#jacobson-radical) is $J(R)=\bigcap_L L$, where $L$ runs over the [maximal right ideals](../../../associative-algebra.md#maximal-right-ideal). Every proper [right ideal](../../../associative-algebra.md#right-ideal) $I$ lies in such an $L$: the union of a chain of proper [right ideals](../../../associative-algebra.md#right-ideal) containing $I$ is a [right ideal](../../../associative-algebra.md#right-ideal) and remains proper because it omits $1$. Thus [Zorn lemma](../../../set-theory.md#zorn-s-lemma) applies.

The right-module form of [Nakayama lemma](../../../mathematics.md#nakayama-lemma) says that a [finitely generated module](../../../module-theory.md#finitely-generated-module) $M$ with $MJ=M$ is zero. More generally, if $N$ is a [submodule](../../../module-theory.md#submodule) and $M=N+MJ$, then $M=N$. To prove the first statement, suppose $M\ne0$ and take a generating set $m_1,\ldots,m_s$ of minimal size. Since $MJ=M$, there are $a_i\in J$ with

$$
m_s=\sum_{i=1}^s m_i a_i,\qquad
m_s(1-a_s)=\sum_{i<s}m_i a_i.
$$

The [unit criterion for the Jacobson radical](../../../noncommutative-algebra.md#unit-criterion-for-the-jacobson-radical) makes $1-a_s$ a [unit](../../../algebra.md#unit-in-a-ring). Hence $m_s$ is generated by the other $m_i$, a contradiction. Apply this result to the [quotient module](../../../module-theory.md#quotient-module) $M/N$ to obtain the general form.

For an [injective](../../../algebra.md#injective-function) [module endomorphism](../../../module-theory.md#module-endomorphism) $f$ of an [Artinian module](../../../module-theory.md#artinian-module) $M$, the [descending chain condition](../../../algebra.md#descending-chain-condition) gives

$$
f^n(M)=f^{n+1}(M)
$$

for some $n$. Given $x\in M$, write $f^n(x)=f^{n+1}(y)$; injectivity of $f^n$ gives $x=f(y)$. Thus $f$ is [surjective](../../../algebra.md#surjective-function), as asserted by [Artinian modules are co-Hopfian](../../../module-theory.md#artinian-modules-are-co-hopfian).

Now $R$ is a [semilocal ring](../../../noncommutative-algebra.md#semi-local-ring) and $\overline V=V/VJ$ is a [finitely generated module](../../../module-theory.md#finitely-generated-module) over the [right Artinian ring](../../../noncommutative-algebra.md#right-artinian-ring) $\overline R=R/J$. A finite [direct sum](../../../vector-space.md#direct-sum) of copies of $\overline R$, and hence its [quotient module](../../../module-theory.md#quotient-module) $\overline V$, is an [Artinian module](../../../module-theory.md#artinian-module). The [module endomorphism](../../../module-theory.md#module-endomorphism) $\alpha$ induces $\overline\alpha$ on $\overline V$, and the given inverse-image condition says precisely that $\ker\overline\alpha=0$. The preceding argument makes $\overline\alpha$ [surjective](../../../algebra.md#surjective-function), so

$$
V=\alpha(V)+VJ.
$$

The [quotient module](../../../module-theory.md#quotient-module) $W=V/\alpha(V)$ is finitely generated and satisfies $WJ=W$. Applying [Nakayama lemma](../../../mathematics.md#nakayama-lemma) yields $W=0$. Therefore **$\alpha$ is surjective**, by [surjectivity from injectivity modulo the Jacobson radical](../../../noncommutative-algebra.md#surjectivity-from-injectivity-modulo-the-jacobson-radical).

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An [essential right ideal](../../../module-theory.md#essential-right-ideal) intersects every nonzero [right ideal](../../../associative-algebra.md#right-ideal) nontrivially. A [regular element of a ring](../../../noncommutative-algebra.md#regular-element-of-a-ring) is a two-sided [non-zero-divisor](../../../mathematics.md#non-zero-divisor): both $cr=0$ and $rc=0$ imply $r=0$. Writing $S$ for the set of these elements, the [classical right ring of quotients](../../../noncommutative-algebra.md#classical-right-ring-of-quotients) is a [ring](../../../commutative-algebra.md#ring) $Q$ containing $R$, with every $s\in S$ invertible and every element of $Q$ expressible as $as^{-1}$.

[Goldie theorem](../../../noncommutative-algebra.md#goldie-s-theorem) states that a [semiprime ring](../../../noncommutative-algebra.md#semiprime-ring) has a semisimple Artinian [classical right ring of quotients](../../../noncommutative-algebra.md#classical-right-ring-of-quotients) if and only if it is a [right Goldie ring](../../../noncommutative-algebra.md#right-goldie-ring): it satisfies the [ascending chain condition](../../../algebra.md#ascending-chain-condition) on right annihilators and has finite [uniform dimension](../../../module-theory.md#uniform-dimension). In particular, every [semiprime ring](../../../noncommutative-algebra.md#semiprime-ring) that is a [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring) satisfies the theorem. We prove the requested case directly using the supplied assumption about [essential right ideals](../../../module-theory.md#essential-right-ideal).

First let $c\in S$. If a nonzero [right ideal](../../../associative-algebra.md#right-ideal) $B$ had $B\cap cR=0$, the sum

$$
B+cB+c^2B+\cdots
$$

would be direct. Indeed, a finite relation $b_0+cb_1+\cdots+c^mb_m=0$ gives $b_0\in B\cap cR$, hence $b_0=0$; cancellation of $c$ repeats the argument. Each $c^jB$ is a nonzero [right ideal](../../../associative-algebra.md#right-ideal), so the partial sums form a strictly ascending chain. This contradicts [right Noetherianity](../../../noncommutative-algebra.md#right-noetherian-ring). Thus [a regular principal right ideal in a right Noetherian ring is essential](../../../module-theory.md#a-regular-principal-right-ideal-in-a-right-noetherian-ring-is-essential), and every [right ideal](../../../associative-algebra.md#right-ideal) containing $c$ is essential.

For $r\in R$ and $c\in S$, put

$$
E=\{x\in R:rx\in cR\}.
$$

This is an [essential right ideal](../../../module-theory.md#essential-right-ideal). To check this, take a nonzero [right ideal](../../../associative-algebra.md#right-ideal) $B$. If $rB=0$, then $B\subseteq E$. Otherwise $rB$ is a nonzero [right ideal](../../../associative-algebra.md#right-ideal), so it meets $cR$ nontrivially; lifting an element of that intersection gives a nonzero element of $B\cap E$. By the supplied assumption, $E$ contains some $d\in S$, giving

$$
rd=cb\qquad\text{for some }b\in R.
$$

This is the [right Ore condition](../../../noncommutative-algebra.md#right-ore-condition). The set $S$ is multiplicatively closed, and the denominator cancellation condition holds because its elements are [non-zero-divisors](../../../mathematics.md#non-zero-divisor). Therefore [Ore theorem](../../../noncommutative-algebra.md#ore-theorem) constructs $Q$ and embeds $R$ in it.

For every [right ideal](../../../associative-algebra.md#right-ideal) $J$ of $Q$,

$$
J=(J\cap R)Q.
$$

Indeed, if $x=as^{-1}\in J$, then $a=xs\in J\cap R$. Contracting an ascending chain of [right ideals](../../../associative-algebra.md#right-ideal) of $Q$ to $R$ therefore proves that $Q$ is a [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring).

Suppose $J$ is an [essential right ideal](../../../module-theory.md#essential-right-ideal) of $Q$. For a nonzero [right ideal](../../../associative-algebra.md#right-ideal) $B$ of $R$, choose $0\ne x\in J\cap BQ$. The [right Ore condition](../../../noncommutative-algebra.md#right-ore-condition) gives a common right denominator for a finite expression of $x$ in $BQ$, so there is $s\in S$ with

$$
0\ne xs\in B\cap(J\cap R).
$$

Thus $J\cap R$ is an [essential right ideal](../../../module-theory.md#essential-right-ideal) of $R$. It contains a [regular element of a ring](../../../noncommutative-algebra.md#regular-element-of-a-ring), which becomes a [unit](../../../algebra.md#unit-in-a-ring) in $Q$, and consequently $J=Q$.

Finally, for any [right ideal](../../../associative-algebra.md#right-ideal) $A$ of $Q$, choose by [Zorn lemma](../../../set-theory.md#zorn-s-lemma) a [right ideal](../../../associative-algebra.md#right-ideal) $B$ maximal subject to $A\cap B=0$. Then $A\oplus B$ is essential: a nonzero [right ideal](../../../associative-algebra.md#right-ideal) disjoint from $A+B$ would enlarge $B$ while keeping it disjoint from $A$. Hence $A\oplus B=Q$. Every [submodule](../../../module-theory.md#submodule) of the right regular [module](../../../module-theory.md#module-mathematics) has a complement, making it a [semisimple module](../../../module-theory.md#semisimple-module). Since it is also [Noetherian](../../../algebra.md#noetherian-ring), it is a finite [direct sum](../../../vector-space.md#direct-sum) of [simple modules](../../../module-theory.md#irreducible-module). It is therefore [Artinian](../../../algebra.md#artinian-ring), and $Q$ is a **semisimple Artinian ring**. This is [semisimplicity of a classical quotient from regular elements in essential ideals](../../../noncommutative-algebra.md#semisimplicity-of-a-classical-quotient-from-regular-elements-in-essential-ideals).

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [filtration of a ring](../../../module-theory.md#filtration-of-a-ring) is an exhaustive increasing family of additive subgroups $F_iR$, indexed by the integers, with $1\in F_0R$ and $F_iR\,F_jR\subseteq F_{i+j}R$. A compatible [filtration of a module](../../../module-theory.md#filtration-of-a-module) on a right [module](../../../module-theory.md#module-mathematics) satisfies $F_iM\,F_jR\subseteq F_{i+j}M$. The [associated graded module](../../../commutative-algebra.md#associated-graded-module) has components $F_iM/F_{i-1}M$, and its action by the [associated graded ring](../../../commutative-algebra.md#associated-graded-ring) is

$$
(m+F_{i-1}M)(r+F_{j-1}R)=mr+F_{i+j-1}M.
$$

Changing either representative changes the product only by an element of $F_{i+j-1}M$, so the action is well-defined.

The [subspace filtration](../../../module-theory.md#subspace-filtration) on $N$ is $F_iN=N\cap F_iM$. The [quotient filtration](../../../module-theory.md#quotient-filtration) is $F_i(M/N)=(F_iM+N)/N$. Inclusion induces an [injective](../../../algebra.md#injective-function) map $\operatorname{gr}N\to\operatorname{gr}M$, and the quotient induces a [surjective](../../../algebra.md#surjective-function) map to $\operatorname{gr}(M/N)$. If $m\in F_iM$ maps to zero in its degree-$i$ quotient, write $m=n+m'$ with $n\in N$ and $m'\in F_{i-1}M$. Then $n\in N\cap F_iM$, so the kernel is exactly the image of $\operatorname{gr}N$. We have the [short exact sequence](../../../module-theory.md#short-exact-sequence)

$$
\boxed{0\longrightarrow\operatorname{gr}N
\longrightarrow\operatorname{gr}M
\longrightarrow\operatorname{gr}(M/N)\longrightarrow0},
$$

which is [exactness of associated graded modules for induced filtrations](../../../commutative-algebra.md#exactness-of-associated-graded-modules-for-induced-filtrations).

For the negative case, $F_iR=R$ for $i\geq0$. Completeness means that $R\to\varprojlim_q R/F_{-q}R$ is an [isomorphism](../../../algebra.md#isomorphism); in particular the [filtration of a ring](../../../module-theory.md#filtration-of-a-ring) is separated. If $x\in F_{-1}R$ and $r\in R$, then $(xr)^q\in F_{-q}R$. The [geometric series](../../../real-analysis.md#geometric-series)

$$
\sum_{q=0}^{\infty}(xr)^q
$$

converges in the [complete negative filtration](../../../module-theory.md#complete-negative-filtration) and is a two-sided inverse of $1-xr$, by the finite geometric identity and continuity of multiplication. The [unit criterion for the Jacobson radical](../../../noncommutative-algebra.md#unit-criterion-for-the-jacobson-radical) now gives

$$
\boxed{F_{-1}R\subseteq J(R)}.
$$

Let $I$ be any [right ideal](../../../associative-algebra.md#right-ideal). The [associated graded module](../../../commutative-algebra.md#associated-graded-module) $\operatorname{gr}I$ for its [subspace filtration](../../../module-theory.md#subspace-filtration) is a [homogeneous ideal](../../../commutative-algebra.md#homogeneous-ideal) on the right in $\operatorname{gr}R$. If $\operatorname{gr}R$ is a [right Noetherian ring](../../../noncommutative-algebra.md#right-noetherian-ring), choose homogeneous generators that lift to $x_1,\ldots,x_s\in I$, with degrees $d_1,\ldots,d_s\leq0$.

For $x\in I\cap F_dR$, cancel its degree-$d$ symbol by a sum $\sum_i x_i a_{i,0}$ with $a_{i,0}\in F_{d-d_i}R$. The remainder belongs to $I\cap F_{d-1}R$. Repeat the cancellation in each succeeding degree. After $q$ steps,

$$
x-\sum_i x_i\sum_{j=0}^{q-1}a_{i,j}\in F_{d-q}R,
\qquad a_{i,j}\in F_{d-j-d_i}R.
$$

For every $i$, the coefficient series converges to some $a_i\in R$ by completeness. Passing to the limit gives $x=\sum_i x_i a_i$. Thus these finitely many $x_i$ generate the actual [right ideal](../../../associative-algebra.md#right-ideal) $I$; no assumption that $I$ is closed is needed. Since every [right ideal](../../../associative-algebra.md#right-ideal) is finitely generated, **$R$ is right Noetherian**, by [complete negative filtered-graded transfer of Noetherianity](../../../module-theory.md#complete-negative-filtered-graded-transfer-of-noetherianity).

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

The [prime radical of a noncommutative ring](../../../noncommutative-algebra.md#prime-radical-of-a-noncommutative-ring) is $N(R)=\bigcap_P P$, with $P$ ranging over all [prime ideals of a noncommutative ring](../../../noncommutative-algebra.md#prime-ideal-of-a-noncommutative-ring). Here primeness means that for two-sided [ideals](../../../commutative-algebra.md#ideal) $A,B$, $AB\subseteq P$ implies $A\subseteq P$ or $B\subseteq P$. A [minimal prime over an ideal](../../../commutative-algebra.md#minimal-prime-over-an-ideal) $I$ is a [prime ideal](../../../commutative-algebra.md#prime-ideal) containing $I$ with no strictly smaller [prime ideal](../../../commutative-algebra.md#prime-ideal) containing $I$.

The [ascending chain condition](../../../algebra.md#ascending-chain-condition) on [left ideals](../../../associative-algebra.md#left-ideal) also applies to two-sided [ideals](../../../commutative-algebra.md#ideal). We first prove by [Noetherian induction](../../../algebra.md#noetherian-induction) that every proper $I$ contains a finite product of [prime ideals](../../../commutative-algebra.md#prime-ideal), each containing $I$. If there were counterexamples, choose a maximal one. It is not prime, so there are strictly larger two-sided [ideals](../../../commutative-algebra.md#ideal) $A,B$ with $AB\subseteq I$. Neither is a counterexample; products of [prime ideals](../../../commutative-algebra.md#prime-ideal) contained in $A$ and in $B$ then concatenate to a product contained in $I$, a contradiction.

Write $P_1\cdots P_t\subseteq I\subseteq P_j$. Every [prime ideal](../../../commutative-algebra.md#prime-ideal) $P$ over $I$ contains at least one $P_j$, by primeness. The inclusion-minimal members of the finite list $P_j$ are therefore precisely the [minimal primes over an ideal](../../../commutative-algebra.md#minimal-prime-over-an-ideal) $I$: any smaller prime over $I$ would contain a member of that same list. Consequently there are finitely many. Replacing each factor $P_j$ by a minimal prime contained in it gives

$$
Q_1Q_2\cdots Q_t\subseteq I
$$

with each $Q_j$ minimal over $I$. Repeated factors may be necessary; in $k[\varepsilon]/(\varepsilon^m)$ the sole minimal prime $(\varepsilon)$ requires its $m$th power to reach zero.

Apply this to $I=0$. Since $N(R)\subseteq Q_j$ for every $j$,

$$
\boxed{N(R)^t\subseteq Q_1\cdots Q_t=0}.
$$

Thus the [prime radical](../../../noncommutative-algebra.md#prime-radical-of-a-noncommutative-ring) is a [nilpotent ideal](../../../commutative-algebra.md#nilpotent-ideal), as in [finite minimal primes and nilpotent prime radical](../../../noncommutative-algebra.md#finite-minimal-primes-and-nilpotent-prime-radical).

Now assume $R$ is commutative. A [prime ideal](../../../commutative-algebra.md#prime-ideal) $P$ is an [associated prime of a module](../../../module-theory.md#associated-prime-of-a-module) $M$ when $P=\operatorname{Ann}_R(m)$ for some $0\ne m\in M$. Every nonzero [module](../../../module-theory.md#module-mathematics) over $R$ has an associated prime: the [ascending chain condition](../../../algebra.md#ascending-chain-condition) gives a maximal annihilator of a nonzero element, and [maximal annihilator of a module element is prime](../../../module-theory.md#maximal-annihilator-of-a-module-element-is-prime).

Since the given $M$ is a [Noetherian module](../../../algebra.md#noetherian-module), repeatedly choosing such a cyclic [submodule](../../../module-theory.md#submodule) in the next quotient yields a finite [prime filtration](../../../algebra.md#prime-filtration)

$$
0=M_0\subsetneq M_1\subsetneq\cdots\subsetneq M_s=M,
\qquad M_i/M_{i-1}\cong R/P_i.
$$

The process terminates by the [ascending chain condition](../../../algebra.md#ascending-chain-condition). In a [short exact sequence](../../../module-theory.md#short-exact-sequence) $0\to U\to M\to W\to0$, one has $\operatorname{Ass}(M)\subseteq\operatorname{Ass}(U)\cup\operatorname{Ass}(W)$. Indeed, if $P=\operatorname{Ann}(m)$ and $Rm\cap U=0$, the image of $m$ in $W$ still has annihilator $P$. Otherwise choose $0\ne am\in U$; then $a\notin P$, and primeness gives $\operatorname{Ann}(am)=P$. As $\operatorname{Ass}(R/P_i)=\{P_i\}$, induction along the [prime filtration](../../../algebra.md#prime-filtration) proves

$$
\boxed{\operatorname{Ass}_R(M)\subseteq\{P_1,\ldots,P_s\}}.
$$

In particular there are only finitely many [associated primes of a module](../../../module-theory.md#associated-prime-of-a-module).

Finally let $P$ be a [minimal prime ideal](../../../commutative-algebra.md#minimal-prime-ideal) of $R$. Its [localization at a prime ideal](../../../commutative-algebra.md#localization-at-a-prime-ideal) $R_P$ has exactly one prime, its [maximal ideal](../../../commutative-algebra.md#maximal-ideal) $PR_P$. The preceding nilpotence result makes this maximal ideal nilpotent. Choose $0\ne y\in R_P$ annihilated by $PR_P$, for example a nonzero element in its last nonzero power, or $1$ if $PR_P=0$. Since elements outside the maximal ideal are [units](../../../algebra.md#unit-in-a-ring), $\operatorname{Ann}_{R_P}(y)=PR_P$.

Write $y=r/s$. The element $r/1$ is nonzero and also has annihilator $PR_P$. Generate $P$ by $p_1,\ldots,p_\ell$. For each $i$, choose $u_i\notin P$ with $u_ip_ir=0$, and put $u=\prod_i u_i$. Then $m=ur$ remains nonzero after localization, while $Pm=0$. If $am=0$, localization forces $a/1\in PR_P$, and hence $a\in P$. Therefore $\operatorname{Ann}_R(m)=P$. This proves that [minimal primes are associated primes](../../../module-theory.md#minimal-primes-are-associated-primes).

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

Fix a finite-dimensional nonnegative [filtration of a ring](../../../module-theory.md#filtration-of-a-ring) giving $R$ its [almost commutative algebra](../../../module-theory.md#almost-commutative-algebra) structure, and choose a [good filtration of a module](../../../module-theory.md#good-filtration-of-a-module) on $M$. When $\operatorname{gr}R$ is a [standard graded algebra](../../../commutative-algebra.md#standard-graded-algebra), the [Hilbert-Serre theorem](../../../commutative-algebra.md#hilbert-serre-theorem) makes the cumulative Hilbert function $h_M(j)=\dim_k F_jM$ eventually a [polynomial](../../../polynomial.md). For $M\ne0$, define the [dimension of a filtered module](../../../module-theory.md#dimension-of-a-filtered-module) and [multiplicity of a filtered module](../../../module-theory.md#multiplicity-of-a-filtered-module) by

$$
\boxed{d(M)=\deg h_M,\qquad
m(M)=d(M)!\,[j^{d(M)}]h_M(j)}.
$$

Use $d(0)=-\infty$ and $m(0)=0$. With positive weighted generators instead of a standard grading, the cumulative Hilbert function is eventually a [quasipolynomial](../../../commutative-algebra.md#quasipolynomial) with a common positive leading coefficient across residue classes. Equivalently, $h_M(j)=c j^d+O(j^{d-1})$, and the definitions are $d(M)=d$ and $m(M)=d!\,c$. The common leading coefficient follows from monotonicity: interlacing consecutive residue classes forces their leading coefficients to agree. For a standard grading, multiplicity is a positive integer, since an integer-valued [polynomial](../../../polynomial.md) has an integral expansion in the binomial polynomials; weighted normalization can instead give a positive rational number.

Two [good filtrations of a module](../../../module-theory.md#good-filtration-of-a-module) for this fixed algebra filtration bound each other after fixed index shifts. The corresponding Hilbert functions therefore satisfy $h_F(j-a)\leq h_G(j)\leq h_F(j+b)$ for fixed $a,b$. Comparing their leading growth shows that the degree and leading coefficient agree. Thus $d(M)$ and $m(M)$ are independent of the module filtration; the fixed algebra filtration is part of the multiplicity convention.

For a [submodule](../../../module-theory.md#submodule) $N$, use its [subspace filtration](../../../module-theory.md#subspace-filtration) and the [quotient filtration](../../../module-theory.md#quotient-filtration) on $M/N$. These are good because $\operatorname{gr}R$ is [Noetherian](../../../algebra.md#noetherian-ring). The [short exact sequence](../../../module-theory.md#short-exact-sequence) of filtered pieces gives

$$
h_M(j)=h_N(j)+h_{M/N}(j).
$$

Nonzero leading coefficients are positive, so

$$
\boxed{d(M)=\max\{d(N),d(M/N)\}}.
$$

If $d(N)=d(M/N)$, those leading coefficients add and

$$
\boxed{m(M)=m(N)+m(M/N)}.
$$

This is [dimension and multiplicity in a filtered exact sequence](../../../module-theory.md#dimension-and-multiplicity-in-a-filtered-exact-sequence).

For the [Weyl algebra](../../../noncommutative-algebra.md#weyl-algebra) $A_n(k)$ in characteristic zero, [Bernstein inequality for Weyl algebra modules](../../../associative-algebra.md#bernstein-inequality-for-weyl-algebra-modules) asserts $d(M)\geq n$ for every nonzero [finitely generated module](../../../module-theory.md#finitely-generated-module) $M$. Write its generators as $x_i,D_i$, with $[D_i,x_j]=\delta_{ij}$ and all other generator commutators zero. The ordered monomials $x^\alpha D^\beta$ give the [Bernstein filtration](../../../noncommutative-algebra.md#bernstein-filtration)

$$
A_j=\operatorname{span}_k\{x^\alpha D^\beta:|\alpha|+|\beta|\leq j\},
\qquad\dim_k A_j=\binom{j+2n}{2n}.
$$

Take a finite-dimensional generating subspace $V\ne0$ of $M$ and put $M_j=A_jV$.

To prove [faithful finite-step action of a Weyl algebra](../../../associative-algebra.md#faithful-finite-step-action-of-a-weyl-algebra), consider $0\ne a\in A_j$ and choose a nonzero coefficient $c_{\alpha\beta}$ of a monomial of maximal total degree $d\leq j$. Applying $\prod_i(\operatorname{ad}D_i)^{\alpha_i}(\operatorname{ad}x_i)^{\beta_i}$ to $a$ gives

$$
\lambda=c_{\alpha\beta}\alpha!\,\beta!\,(-1)^{|\beta|}\ne0.
$$

Indeed, these [commutators](../../../lie-algebra.md#commutator) differentiate the ordered coefficients: lower-degree monomials vanish, and another degree-$d$ monomial can survive only if all its exponents dominate $(\alpha,\beta)$, which forces equality. This is [scalar extraction by iterated Weyl commutators](../../../associative-algebra.md#scalar-extraction-by-iterated-weyl-commutators).

Expanding these iterated [commutators](../../../lie-algebra.md#commutator) writes $\lambda=\sum_\ell u_\ell a v_\ell$ with $u_\ell,v_\ell\in A_j$. If $a$ annihilated $M_j$, every summand would annihilate $V$, contrary to $\lambda V\ne0$. Therefore the action map is [injective](../../../algebra.md#injective-function):

$$
A_j\hookrightarrow\operatorname{Hom}_k(M_j,M_{2j}).
$$

Taking dimensions and comparing polynomial degrees gives

$$
\binom{j+2n}{2n}\leq h_M(j)h_M(2j),
\qquad 2n\leq2d(M),
$$

which proves [Bernstein inequality for Weyl algebra modules](../../../associative-algebra.md#bernstein-inequality-for-weyl-algebra-modules). The polynomial representation $k[x_1,\ldots,x_n]$ has dimension $n$, so the bound is sharp.

The [associated graded ring](../../../commutative-algebra.md#associated-graded-ring) of the [Weyl algebra](../../../noncommutative-algebra.md#weyl-algebra) is a polynomial ring, so [ascending filtered-graded transfer of Noetherianity](../../../module-theory.md#ascending-filtered-graded-transfer-of-noetherianity) makes $A_n(k)$ a [left Noetherian ring](../../../noncommutative-algebra.md#left-noetherian-ring). Thus every [submodule](../../../module-theory.md#submodule) of a [finitely generated module](../../../module-theory.md#finitely-generated-module) is finitely generated. If $d(M)=n$, every nonzero subquotient has dimension at most $n$ by the exact-sequence formula, and at least $n$ by [Bernstein inequality for Weyl algebra modules](../../../associative-algebra.md#bernstein-inequality-for-weyl-algebra-modules). Every such subquotient therefore has dimension $n$ and positive integral multiplicity.

In a strictly descending chain $M=M_0\supsetneq M_1\supsetneq\cdots$, each nonzero quotient $M_i/M_{i+1}$ consumes at least one unit of multiplicity, by [dimension and multiplicity in a filtered exact sequence](../../../module-theory.md#dimension-and-multiplicity-in-a-filtered-exact-sequence). Hence there are at most $m(M)$ strict steps. This proves the [descending chain condition](../../../algebra.md#descending-chain-condition), so **$M$ is Artinian**. In fact this [holonomic Weyl algebra module](../../../associative-algebra.md#holonomic-weyl-algebra-module) has [module length](../../../module-theory.md#length-of-a-module) at most $m(M)$, as in [multiplicity bounds the length of a holonomic Weyl module](../../../associative-algebra.md#multiplicity-bounds-the-length-of-a-holonomic-weyl-module).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
