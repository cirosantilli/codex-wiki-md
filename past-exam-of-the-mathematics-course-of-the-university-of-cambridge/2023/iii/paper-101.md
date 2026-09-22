# Paper 101

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_101.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_101.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
    - [iv](#1/a/iv)
      - [Solution](#1/a/iv/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [i](#4/d/i)
      - [Solution](#4/d/i/solution)
    - [ii](#4/d/ii)
      - [Solution](#4/d/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)
    - [iii](#5/c/iii)
      - [Solution](#5/c/iii/solution)
    - [iv](#5/c/iv)
      - [Solution](#5/c/iv/solution)
    - [v](#5/c/v)
      - [Solution](#5/c/v/solution)

## 1

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

**False.** The [integers](../../../number-theory.md#integer) $\mathbb Z$ form a [Noetherian ring](../../../algebra.md#noetherian-ring), since every [ideal](../../../commutative-algebra.md#ideal) is [principal](../../../commutative-algebra.md#principal-ideal), but this ring is not an [Artinian ring](../../../algebra.md#artinian-ring): the strictly descending chain

$$
(2)\supsetneq(2^2)\supsetneq(2^3)\supsetneq\cdots
$$

never stabilizes.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

**True.** This is the [Artinian commutative ring is Noetherian theorem](../../../algebra.md#artinian-commutative-ring-is-noetherian-theorem). One proof uses the nilpotent [nilradical](../../../commutative-algebra.md#nilradical) $N$ of an [Artinian ring](../../../algebra.md#artinian-ring) $A$. The quotient $A/N$ is a finite product of [fields](../../../algebra.md#field). Each quotient $N^j/N^{j+1}$ is an Artinian module over the [semisimple ring](../../../commutative-algebra.md#semisimple-ring) $A/N$, hence has [finite length](../../../module-theory.md#length-of-a-module) and is [Noetherian](../../../algebra.md#noetherian-module). The finite filtration

$$
A\supseteq N\supseteq\cdots\supseteq N^r=0
$$

then makes $A$ a Noetherian module over itself, which is exactly the [ascending chain condition](../../../algebra.md#ascending-chain-condition) on its ideals.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

**False.** The [module over a ring](../../../module-theory.md#module-mathematics) $\mathbb Z$ over itself is [Noetherian](../../../algebra.md#noetherian-module), because its submodules are the [principal ideals](../../../commutative-algebra.md#principal-ideal) $n\mathbb Z$, but the descending chain

$$
2\mathbb Z\supsetneq2^2\mathbb Z\supsetneq2^3\mathbb Z\supsetneq\cdots
$$

shows that it is not an [Artinian module](../../../module-theory.md#artinian-module).

<h4 id="1/a/iv">iv</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/a/iv)

**False.** For a [prime number](../../../number-theory.md#prime-number) $p$, the [Prüfer p-group](../../../group.md#prufer-group) $C_{p^\infty}$ is an Artinian $\mathbb Z$-module: every proper subgroup is a finite [cyclic group](../../../group.md#cyclic-group), so no infinite strictly descending chain of subgroups exists. It is not Noetherian because its cyclic subgroups form the strict ascending chain

$$
\boxed{C_p\subsetneq C_{p^2}\subsetneq C_{p^3}\subsetneq\cdots.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $\mathfrak m$ be the [maximal ideal](../../../commutative-algebra.md#maximal-ideal) and $k=A/\mathfrak m$ the finite [residue field](../../../commutative-algebra.md#residue-field). The maximal ideal of an [Artinian local ring](../../../algebra.md#artinian-local-ring) is [nilpotent](../../../commutative-algebra.md#nilpotent-ideal), so $\mathfrak m^r=0$ for some $r$. Every quotient

$$
\mathfrak m^j/\mathfrak m^{j+1}
$$

is both an Artinian $A$-module and a [vector space](../../../vector-space.md) over $k$. An Artinian vector space is finite-dimensional, hence each quotient is a [finite set](../../../set.md#finite-set). The finite filtration

$$
A\supset\mathfrak m\supset\cdots\supset\mathfrak m^r=0
$$

therefore proves that the underlying set of $A$ is finite. This is the [Finiteness criterion for an Artinian local ring](../../../algebra.md#finiteness-criterion-for-an-artinian-local-ring).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Suppose for a contradiction that $m>n$. Compose the given [injective module homomorphism](../../../module-theory.md#module-homomorphism) with the standard injection $B^n\hookrightarrow B^m$ that appends $m-n$ zero coordinates. This gives an injective [endomorphism](../../../algebra.md#endomorphism) $T$ of the [finite free module](../../../module-theory.md#finite-free-module) $B^m$ whose matrix has a zero final row.

Its [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) has zero constant term, so the [Cayley-Hamilton theorem](../../../mathematics.md#cayley-hamilton-theorem) gives

$$
T^m+c_{m-1}T^{m-1}+\cdots+c_1T=0.
$$

Injectivity lets us cancel $T$. Repeating this argument eventually gives the identity endomorphism equal to zero. That would imply $B^m=0$, contrary to $B\ne0$. Hence $m\leq n$. This proves the [rank inequality for an injection of finite free modules](../../../module-theory.md#rank-inequality-for-an-injection-of-finite-free-modules).

## 2

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

A [ring extension](../../../commutative-algebra.md#ring-extension) $A\subseteq B$ is an [integral extension](../../../commutative-algebra.md#integral-extension) when every $b\in B$ is an [integral element](../../../commutative-algebra.md#integral-element) over $A$: there is a [monic polynomial](../../../polynomial.md#monic-polynomial)

$$
b^d+a_{d-1}b^{d-1}+\cdots+a_0=0
$$

with all $a_i\in A$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

A [ring extension](../../../commutative-algebra.md#ring-extension) $A\subseteq B$ is [finite](../../../commutative-algebra.md#module-finite-ring-extension) when $B$ is a [finitely generated module](../../../module-theory.md#finitely-generated-module) over $A$. Every finite extension is integral by the [determinant trick](../../../module-theory.md#determinant-trick).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [prime ideal correspondence for localization](../../../commutative-algebra.md#prime-ideal-correspondence-for-localization) identifies primes of $B_{\mathfrak p}$ with primes $\mathfrak q$ of $B$ disjoint from $A\setminus\mathfrak p$. Passing to the quotient by $\mathfrak pB_{\mathfrak p}$ retains exactly those containing $\mathfrak pB_{\mathfrak p}$. Thus the image is the [fiber of the map on spectra](../../../commutative-algebra.md#fiber-of-the-map-on-spectra):

$$
\boxed{\left\{\mathfrak q\in\operatorname{Spec}B:\mathfrak q\cap A=\mathfrak p\right\}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The claim fails for a general extension. If $k$ is an infinite [field](../../../algebra.md#field), all the infinitely many maximal ideals $(x-a)$ of $k[x]$ contract to $(0)$ in $k$.

It still fails for an [integral extension](../../../commutative-algebra.md#integral-extension). Take a finite field $k=\mathbb F_q$ and

$$
B=\prod_{j\geq1}k.
$$

Every $b\in B$ satisfies the monic equation $b^q-b=0$, so $B$ is integral over the diagonal copy of $k$. The coordinate kernels are infinitely many distinct [maximal ideals](../../../commutative-algebra.md#maximal-ideal), all lying over $(0)$.

**The claim is true for a [module-finite ring extension](../../../commutative-algebra.md#module-finite-ring-extension).** The primes above $\mathfrak p$ correspond to the primes of the [fiber ring](../../../commutative-algebra.md#fiber-ring)

$$
B\otimes_A\kappa(\mathfrak p).
$$

This is a finite-dimensional algebra over the [residue field](../../../commutative-algebra.md#residue-field) $\kappa(\mathfrak p)$, hence an [Artinian ring](../../../algebra.md#artinian-ring), and an Artinian ring has only finitely many prime ideals.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Form the finite-dimensional $k$-algebra

$$
C=B\otimes_{A,f}k.
$$

Because a finite extension is integral, the [Lying-over theorem](../../../commutative-algebra.md#lying-over-theorem) supplies a prime of $B$ above $\ker f$; after localization and extension of the residue field to $k$, this shows $C\ne0$. Therefore $C$ has at least one [maximal ideal](../../../commutative-algebra.md#maximal-ideal).

As an [Artinian ring](../../../algebra.md#artinian-ring), $C$ has only finitely many maximal ideals. For each such ideal $\mathfrak n$, the quotient $C/\mathfrak n$ is a finite [field extension](../../../algebra.md#field-extension) of the algebraically closed field $k$, so it equals $k$. Consequently the quotient maps $C\to k$ are in bijection with the required extensions $g:B\to k$. The set of extensions is therefore finite and nonempty.

## 3

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

[Zariski lemma](../../../algebraic-geometry.md#zariski-s-lemma) says that a field which is a [finitely generated algebra](../../../algebra.md#finitely-generated-algebra) over a field $k$ is a finite algebraic extension of $k$. The [Strong Hilbert Nullstellensatz](../../../algebraic-geometry.md#strong-hilbert-nullstellensatz) says that, for an ideal $I\subseteq k[T_1,\ldots,T_n]$ over an [algebraically closed field](../../../algebra.md#algebraically-closed-field),

$$
I(V(I))=\sqrt I.
$$

Let the unique point of $V(\mathfrak a)$ be $x=(x_1,\ldots,x_n)$ and let

$$
\mathfrak m=(T_1-x_1,\ldots,T_n-x_n).
$$

The Nullstellensatz gives $\sqrt{\mathfrak a}=\mathfrak m$, so $\mathfrak a\subseteq\mathfrak m$. Each of the finitely many generators $u_i=T_i-x_i$ of $\mathfrak m$ has some power $u_i^{e_i}\in\mathfrak a$. If

$$
r=1+\sum_i(e_i-1),
$$

then every monomial of total degree $r$ in the $u_i$ is divisible by one of the $u_i^{e_i}$. Hence

$$
\mathfrak m^r\subseteq\mathfrak a\subseteq\mathfrak m.
$$

**Thus the assertion is true; algebraically, the quotient defines a [punctual scheme](../../../ringed-space.md#punctual-scheme) supported at $x$.**

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose finite generating sets $I=(g_1,\ldots,g_s)$ and $J=(f_1,\ldots,f_t)$, using the [Hilbert basis theorem](../../../algebra.md#hilbert-basis-theorem). The assumed inclusion says that each $f_j$ vanishes on $V_{\mathbb C}(I)$. By the [Strong Hilbert Nullstellensatz](../../../algebraic-geometry.md#strong-hilbert-nullstellensatz), for every $j$ there is an exponent $N_j$ such that

$$
f_j^{N_j}\in I\mathbb C[T_1,\ldots,T_n].
$$

The coefficients in an expression $f_j^{N_j}=\sum_iq_{ij}g_i$ solve a finite [system of linear equations](../../../linear-algebra.md#system-of-linear-equations) with rational coefficients. Since it has a complex solution, [Gaussian elimination](../../../numerical-analysis.md#gaussian-elimination) gives a rational solution. Clearing the finitely many denominators produces a nonzero integer $D$ such that

$$
D f_j^{N_j}\in I
$$

for every $j$.

For any prime $p\nmid D$, reduce these identities modulo $p$. At a common zero of $\pi_p(I)$ in the [algebraic closure](../../../algebra.md#algebraic-closure) $\overline{\mathbb F}_p$, they give $\pi_p(f_j)^{N_j}=0$, hence $\pi_p(f_j)=0$, for all $j$. Therefore

$$
V_{\overline{\mathbb F}_p}(\pi_p(I))
\subseteq
V_{\overline{\mathbb F}_p}(\pi_p(J))
$$

for every prime except the finitely many divisors of $D$. This is the [spreading out of an affine zero-set inclusion](../../../algebraic-geometry.md#spreading-out-of-an-affine-zero-set-inclusion).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

An $A$-module $M$ is a [flat module](../../../module-theory.md#flat-module) when the [tensor functor](../../../module-theory.md#tensor-product-of-modules) $-\otimes_AM$ preserves injections, equivalently when it is exact.

Suppose first that $M$ is flat. For any nonzero $a\in A$, tensor the injection $A\xrightarrow{a}A$ with $M$. The resulting map $M\xrightarrow{a}M$ is injective, so $am=0$ implies $m=0$. Thus $M$ is a [torsion-free module](../../../module-theory.md#torsion-free-module).

Conversely, suppose $M$ is torsion-free over the [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain) $A$. Every finitely generated submodule of $M$ is a finitely generated torsion-free module over a PID, hence a [finite free module](../../../module-theory.md#finite-free-module) and therefore flat. The module $M$ is the [filtered colimit](../../../module-theory.md#filtered-colimit-of-modules) of these submodules. Tensor products commute with filtered colimits, and filtered colimits of modules preserve exact sequences, so $M$ is flat. This proves that a [torsion-free module over a principal ideal domain is flat](../../../module-theory.md#torsion-free-module-over-a-principal-ideal-domain-is-flat).

## 4

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Suppose $xy\in J$ and $x\notin J$. Then the [colon ideal](../../../commutative-algebra.md#colon-ideal) $(J:x)$ properly contains $J$ because it contains $y$. If also $y\notin J$, then $J+(x)$ properly contains $J$. The maximality of $J$ in the family makes both larger ideals lie outside the family. Applying the stated closure condition with $I=J$ and $a=x$ would imply $J$ lies outside the family, a contradiction. Hence $x\in J$ or $y\in J$, and $J$ is a [prime ideal](../../../commutative-algebra.md#prime-ideal). This argument is the [Prime ideal principle for an Oka family](../../../commutative-algebra.md#prime-ideal-principle-for-an-oka-family).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $\mathcal F$ be the proper nonprincipal ideals. A chain in $\mathcal F$ has a nonprincipal union: if its union were $(a)$, then $a$ would belong to one member of the chain, forcing that member to equal the union and be principal. The union is also proper. Thus [Zorn lemma](../../../set-theory.md#zorn-s-lemma) gives a maximal member whenever $\mathcal F$ is nonempty.

The family satisfies the condition from part (a). Indeed, suppose

$$
I+(a)=(b),\qquad (I:a)=(c).
$$

Write $a=bd$ and $b=i+ra$, where $i\in I$. Every $x=bs\in I$ has $as=dx\in I$, so $s\in(c)$ and $I\subseteq(bc)$. Conversely $ac\in I$ because $c\in(I:a)$, while $ic\in I$ because $i\in I$. Thus $bc=ic+rac\in I$, proving $(bc)\subseteq I$. Hence $I=(bc)$ is principal.

If a nonprincipal ideal existed, part (a) would therefore produce a nonprincipal prime ideal, contrary to the hypothesis. Every ideal is principal, so the [integral domain](../../../commutative-algebra.md#integral-domain) is a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Suppose first that $A$ is a [unique factorization domain](../../../algebra.md#unique-factorization-domain), and let $\mathfrak p$ be a minimal nonzero prime ideal. Choose $0\ne a\in\mathfrak p$ and factor it into [irreducibles](../../../commutative-algebra.md#irreducible-element). In a UFD each irreducible is a [prime element](../../../commutative-algebra.md#prime-element), so one factor $\pi$ belongs to $\mathfrak p$. The nonzero prime ideal $(\pi)\subseteq\mathfrak p$ must equal $\mathfrak p$ by minimality.

Conversely, the [ascending chain condition](../../../algebra.md#ascending-chain-condition) in the Noetherian domain implies that every nonzero nonunit factors into irreducibles. Let $\pi$ be irreducible and choose a prime $\mathfrak p$ minimal over $(\pi)$. The [Krull principal ideal theorem](../../../commutative-algebra.md#krull-principal-ideal-theorem) gives $\operatorname{ht}\mathfrak p\leq1$. Since $A$ is a domain and $\mathfrak p\ne(0)$, it is a minimal nonzero prime and hence is principal, say $\mathfrak p=(q)$. The divisibility $q\mid\pi$ and irreducibility of $\pi$ force $q$ to be associate to $\pi$, so $(\pi)=\mathfrak p$ is prime. Thus every irreducible is prime, proving that $A$ is a UFD. This is the [Minimal-prime criterion for a Noetherian unique factorization domain](../../../algebra.md#minimal-prime-criterion-for-a-noetherian-unique-factorization-domain).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/i">i</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/i/solution">Solution</h5>

↑ **Parent:** [I](#4/d/i)

Let $A$ be a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain) that is not a field. A PID is [Noetherian](../../../algebra.md#noetherian-ring) and is a [unique factorization domain](../../../algebra.md#unique-factorization-domain). Every nonzero prime ideal is generated by a prime element. If

$$
(p)\subseteq(a)\subsetneq A,
$$

then $a\mid p$, so primality of $p$ makes $a$ a unit or an associate of $p$. The proper alternative is $(a)=(p)$, and every nonzero prime is therefore maximal. Since $A$ has a nonzero prime ideal, its [Krull dimension](../../../commutative-algebra.md#krull-dimension) is exactly one.

<h4 id="4/d/ii">ii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/d/ii)

Conversely, let $A$ be a Noetherian UFD of Krull dimension one. Every nonzero prime is minimal among nonzero primes, and the forward argument in part (c) makes it principal. The zero ideal is principal as well, so part (b) shows that $A$ is a PID. A field has Krull dimension zero, hence $A$ is not a field.

## 5

↑ **Parent:** [Paper 101](paper-101.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

This is the [Artin--Tate lemma](../../../algebra.md#artin-tate-lemma). Choose $A$-algebra generators $x_1,\ldots,x_r$ of $C$ and $B$-module generators $e_1,\ldots,e_s$ of $C$. Write

$$
x_i=\sum_j a_{ij}e_j,\qquad
e_ie_j=\sum_\ell b_{ij\ell}e_\ell
$$

with coefficients $a_{ij},b_{ij\ell}\in B$, and let $B_0$ be the $A$-subalgebra of $B$ generated by these finitely many coefficients.

The module $\sum_jB_0e_j$ contains the $x_i$, is closed under multiplication, and contains $A$ after including an expression for $1$ among the chosen coefficients. It therefore equals $C$. Thus $C$ is a finite $B_0$-module. The ring $B_0$ is Noetherian by the [Hilbert basis theorem](../../../algebra.md#hilbert-basis-theorem), and $B\subseteq C$ is a $B_0$-submodule, so $B$ is a finite $B_0$-module. It follows that $B$ is a finitely generated $A$-algebra.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Let $K$ be a field finitely generated as a $\mathbb Z$-algebra. If $K$ has positive [characteristic](../../../algebra.md#characteristic-of-a-field) $p$, it is a finitely generated algebra over $\mathbb F_p$; [Zariski lemma](../../../algebraic-geometry.md#zariski-s-lemma) makes it a finite algebraic extension of the finite field $\mathbb F_p$, so $K$ is finite.

Suppose instead that $K$ has characteristic zero. Then $K$ is a finitely generated $\mathbb Q$-algebra and Zariski lemma makes it a [number field](../../../algebraic-number-theory.md#number-field). For algebra generators $\alpha_1,\ldots,\alpha_r$, choose a nonzero integer $N$ such that every $\alpha_i$ is integral over $\mathbb Z[1/N]$. The whole algebra $K=\mathbb Z[\alpha_1,\ldots,\alpha_r]$ would then be integral over $\mathbb Z[1/N]$. But for a prime $q\nmid N$, the element $1/q\in K$ is not integral over the integrally closed domain $\mathbb Z[1/N]$, a contradiction. Hence every field finitely generated over the integers is finite, and in particular no infinite field has that property.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

The [Poincare series of a graded module](../../../commutative-algebra.md#poincare-series-of-a-graded-module) is

$$
P_A(t)=\sum_{n\geq0}\dim_k(A_n)t^n.
$$

It is the [generating function](../../../commutative-algebra.md#poincare-series-of-a-graded-module) of the [Hilbert function](../../../commutative-algebra.md#hilbert-function) $n\mapsto\dim_kA_n$.

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

A [Hilbert polynomial](../../../algebraic-geometry.md#hilbert-polynomial) of $A$ is a polynomial $h_A(X)\in\mathbb Q[X]$ such that

$$
h_A(n)=\dim_kA_n
$$

for every sufficiently large integer $n$. Eventual equality makes this polynomial unique.

<h4 id="5/c/iii">iii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/c/iii)

Take $A=k[x]$ with $\deg x=2$. This is a Noetherian [graded algebra](../../../commutative-algebra.md#graded-algebra) with $A_0=k$, but

$$
\dim_kA_n=
\begin{cases}
1,&n\ \text{even},\\
0,&n\ \text{odd}.
\end{cases}
$$

**No polynomial can agree eventually with these alternating values, so $A$ has no Hilbert polynomial.**

<h4 id="5/c/iv">iv</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#5/c/iv)

A sufficient condition is that $A$ be a [standard graded algebra](../../../commutative-algebra.md#standard-graded-algebra): it is generated as a $k$-algebra by finitely many elements of degree one. The [Hilbert-Serre theorem](../../../commutative-algebra.md#hilbert-serre-theorem) then makes $P_A(t)$ a rational function whose denominator, after cancellation, is a power of $1-t$. When the eventual Hilbert polynomial is nonzero,

$$
\deg h_A=\operatorname{ord}_{t=1}P_A(t)-1,
$$

where the right side uses the order of the pole at $t=1$.

<h4 id="5/c/v">v</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/v/solution">Solution</h5>

↑ **Parent:** [V](#5/c/v)

The degree-$n$ component is

$$
(A\otimes_kB)_n=\bigoplus_{i+j=n}A_i\otimes_kB_j.
$$

Dimensions therefore satisfy the [Cauchy product](../../../real-analysis.md#cauchy-product) rule, giving

$$
\boxed{P_{A\otimes_kB}(t)=P_A(t)P_B(t).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
