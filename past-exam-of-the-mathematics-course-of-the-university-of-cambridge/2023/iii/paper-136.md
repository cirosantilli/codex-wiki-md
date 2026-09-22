# Paper 136

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_136.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_136.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)

## 1

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $I(L/K)$ be the [inertia group](../../../arithmetic.md#inertia-group) and let $\varphi$ denote [Frobenius](../../../arithmetic.md#frobenius-automorphism) on the residue-field extension. The [Relative Weil group](../../../arithmetic.md#relative-weil-group) is

$$
W(L/K)=\{\sigma\in\operatorname{Gal}(L/K):\bar\sigma=\varphi^n\text{ for some }n\in\mathbb Z\}.
$$

Its [Weil-group topology](../../../arithmetic.md#weil-group-topology) makes $I(L/K)$ an open [profinite group](../../../topological-group.md#profinite-group) with its usual topology and gives $W(L/K)/I(L/K)$ the discrete topology. Thus every inertia coset is an open copy of $I(L/K)$.

Take $L=K^{\mathrm{nr}}$, the [maximal unramified extension](../../../arithmetic.md#maximal-unramified-extension) of $K$. Then

$$
\operatorname{Gal}(L/K)\cong\widehat{\mathbb Z},
\qquad
W(L/K)\cong\mathbb Z.
$$

The subgroup $\{0\}\subset\mathbb Z$ is open in the discrete Weil-group topology, but it is not open in the [profinite topology](../../../topological-group.md#profinite-topology) inherited from $\widehat{\mathbb Z}$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The main theorem of [local class field theory](../../../arithmetic.md#local-class-field-theory) gives a continuous [Local Artin map](../../../arithmetic.md#local-artin-map)

$$
\operatorname{Art}_K:K^\times\longrightarrow
\operatorname{Gal}(K^{\mathrm{ab}}/K)
$$

with dense image, normalized by sending a [uniformizer](../../../commutative-algebra.md#uniformizer) to a chosen [Frobenius](../../../arithmetic.md#frobenius-automorphism). For every finite abelian extension $L/K$, it induces the [Local Artin reciprocity](../../../arithmetic.md#local-artin-reciprocity) isomorphism

$$
K^\times/N_{L/K}(L^\times)\cong\operatorname{Gal}(L/K).
$$

The [existence theorem of local class field theory](../../../arithmetic.md#existence-theorem-of-local-class-field-theory) says that the finite-index open subgroups of $K^\times$ are exactly the [norm subgroups](../../../arithmetic.md#norm-subgroup-of-a-local-field-extension) $N_{L/K}(L^\times)$ for finite abelian extensions $L/K$, and that the extension is uniquely determined inside $K^{\mathrm{ab}}$.

Write $e=e(L/K)$ and $f=f(L/K)$. The valuation of a [field norm](../../../algebraic-number-theory.md#field-norm) satisfies

$$
v_K(N_{L/K}x)=f\,v_L(x),
$$

so the valuation image of the norm subgroup is $f\mathbb Z$. The exact sequence obtained from $v_K:K^\times\to\mathbb Z$ therefore gives

$$
[K^\times:N_{L/K}(L^\times)]
=f\,[\mathcal O_K^\times:N_{L/K}(\mathcal O_L^\times)].
$$

The left side is $[L:K]=ef$ by [Local Artin reciprocity](../../../arithmetic.md#local-artin-reciprocity). Cancelling $f$ proves

$$
\boxed{[\mathcal O_K^\times:N_{L/K}(\mathcal O_L^\times)]=e.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [cyclotomic extension of a p-adic field](../../../arithmetic.md#cyclotomic-extension-of-a-p-adic-field)

$$
L_1=\mathbb Q_p(\zeta_p)
$$

has degree $p-1$, is Galois with group $(\mathbb Z/p\mathbb Z)^\times$, and is [totally ramified](../../../arithmetic.md#totally-ramified-extension). Indeed, $\zeta_p-1$ is a root of the [Eisenstein polynomial](../../../arithmetic.md#eisenstein-polynomial)

$$
\frac{(X+1)^p-1}{X}.
$$

Put $\alpha=\sqrt[p-1]{-p}$. Its polynomial $X^{p-1}+p$ is Eisenstein, so $L_2=\mathbb Q_p(\alpha)$ is totally ramified of degree $p-1$. Every $(p-1)$st root of unity lies in $\mathbb Q_p$ by the [Teichmuller lifts](../../../arithmetic.md#teichmuller-representative), so every root $\omega\alpha$ of this polynomial lies in $L_2$. Hence $L_2/\mathbb Q_p$ is also [Galois](../../../galois-theory.md#finite-galois-extension).

For either $L_i/\mathbb Q_p$, the norm has every possible valuation because the [residue-field degree](../../../arithmetic.md#residue-field-degree) is one. The [norm units in a tamely totally ramified extension](../../../arithmetic.md#norm-units-in-a-tamely-totally-ramified-extension) lie in the principal units $1+p\mathbb Z_p$: reduction of a unit norm is the $(p-1)$st power of its residue, hence is $1$. Part (b) says that this unit norm subgroup has index $p-1$, exactly the index of $1+p\mathbb Z_p$ in $\mathbb Z_p^\times$. Consequently

$$
N_{L_1/\mathbb Q_p}(L_1^\times)
=p^{\mathbb Z}(1+p\mathbb Z_p)
=N_{L_2/\mathbb Q_p}(L_2^\times).
$$

The uniqueness clause in the [existence theorem of local class field theory](../../../arithmetic.md#existence-theorem-of-local-class-field-theory) now gives

$$
\boxed{L_1=L_2.}
$$

## 2

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

One strong form of [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) is this: if $K$ is complete for a [discrete valuation](../../../commutative-algebra.md#discrete-valuation) $v$, $f\in\mathcal O_K[X]$, and $a_0\in\mathcal O_K$ satisfies

$$
v(f(a_0))>2v(f'(a_0)),
$$

then there is a unique root $\alpha$ satisfying

$$
v(\alpha-a_0)>v(f'(a_0)).
$$

Define the [Newton iteration over a valued field](../../../arithmetic.md#newton-iteration-over-a-valued-field)

$$
a_{n+1}=a_n-\frac{f(a_n)}{f'(a_n)}.
$$

Taylor expansion and the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality) show inductively that $v(f'(a_n))=v(f'(a_0))$ and

$$
v(f(a_{n+1}))\geq2v(f(a_n))-2v(f'(a_0)).
$$

Thus the valuations of the corrections $a_{n+1}-a_n$ tend to infinity, so $(a_n)$ is a [Cauchy sequence](../../../real-analysis.md#cauchy-sequence). [Completeness](../../../topological-analysis.md#completeness) gives a limit $\alpha$, and [continuity](../../../calculus.md#continuous-function) gives $f(\alpha)=0$. If $\beta$ is another root in the stated ball, Taylor expansion of $f(\beta)-f(\alpha)$ shows that the linear term has strictly smaller valuation than all higher terms unless $\beta=\alpha$, proving uniqueness.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Every $x\in\mathbb Q_2^\times$ has a unique form $2^nu$ with $n\in\mathbb Z$ and $u\in\mathbb Z_2^\times$. Its square class first records $n\bmod2$. An odd [2-adic unit](../../../arithmetic.md#2-adic-unit) is a square precisely when it is congruent to $1$ modulo $8$: necessity follows by squaring an odd integer, and sufficiency follows from [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) applied in its standard $2$-adic square-root form.

The odd residues $1,3,5,7$ modulo $8$ therefore give four unit square classes. Together with valuation parity this yields

$$
\mathbb Q_2^\times/(\mathbb Q_2^\times)^2
\cong(\mathbb Z/2\mathbb Z)^3.
$$

For example, the classes of $-1$, $2$, and $5$ form a basis of the [square-class group of the 2-adic numbers](../../../arithmetic.md#square-class-group-of-the-2-adic-numbers).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The smallest integer is

$$
k=2.
$$

Indeed, reduction modulo $p$ cannot work: the map $x\mapsto x^p$ is the identity on $\mathbb F_p^\times$, although not every element of $\mathbb Z_p^\times$ is a $p$th power.

For odd $p$, the [p-adic unit group](../../../arithmetic.md#p-adic-unit) decomposes as

$$
\mathbb Z_p^\times\cong\mu_{p-1}\times(1+p\mathbb Z_p).
$$

Raising to the $p$th power is an automorphism on $\mu_{p-1}$. On the principal units, the [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm) identifies it with multiplication by $p$ on $p\mathbb Z_p$, so

$$
(1+p\mathbb Z_p)^p=1+p^2\mathbb Z_p.
$$

Hence whether a unit is a $p$th power is determined exactly by its residue modulo $p^2$. Equivalently,

$$
\alpha\in(\mathbb Z_p^\times)^p
\quad\Longleftrightarrow\quad
\alpha\bmod p^2\in((\mathbb Z/p^2\mathbb Z)^\times)^p.
$$

This is the [pth-power criterion for p-adic units](../../../arithmetic.md#pth-power-criterion-for-p-adic-units).

## 3

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $G=\operatorname{Gal}(L/K)$. The lower [ramification groups](../../../arithmetic.md#ramification-group) are $G_{-1}=G$ and, for $i\geq0$,

$$
G_i=\{\sigma\in G:v_L(\sigma(x)-x)\geq i+1
\text{ for every }x\in\mathcal O_L\}.
$$

If $L/K$ is totally ramified and $\pi_L$ is a [uniformizer](../../../commutative-algebra.md#uniformizer), then $\mathcal O_L=\mathcal O_K[\pi_L]$. Factoring $F(\sigma\pi_L)-F(\pi_L)$ by $\sigma\pi_L-\pi_L$ for $F\in\mathcal O_K[X]$ proves the [uniformizer criterion for lower ramification groups](../../../arithmetic.md#uniformizer-criterion-for-lower-ramification-groups)

$$
G_i=\{\sigma\in G:v_L(\sigma(\pi_L)-\pi_L)\geq i+1\}.
$$

For $\sigma\in G_0$, define

$$
\theta(\sigma)=\overline{\frac{\sigma(\pi_L)}{\pi_L}}\in k_L^\times.
$$

The [inertia group](../../../arithmetic.md#inertia-group) $G_0$ acts trivially on $k_L$, so $\theta(\sigma\tau)=\theta(\sigma)\theta(\tau)$. Its kernel consists exactly of those $\sigma$ for which $\sigma(\pi_L)/\pi_L\equiv1$ modulo the maximal ideal, namely $G_1$. The [first isomorphism theorem](../../../group-theory.md#first-isomorphism-theorem) therefore gives an injection

$$
\boxed{G_0/G_1\hookrightarrow k_L^\times.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $\alpha$ be a root of

$$
f(X)=X^3+3X+3.
$$

The polynomial is Eisenstein at $3$, so $E=\mathbb Q_3(\alpha)$ is totally ramified of degree three and $\mathcal O_E=\mathbb Z_3[\alpha]$. Its discriminant is

$$
\Delta=-4\cdot3^3-27\cdot3^2=-351=-3^3\cdot13.
$$

Its odd valuation makes $\Delta$ nonsquare in $\mathbb Q_3$, so the [Galois group of an irreducible cubic](../../../galois-theory.md#galois-group-of-an-irreducible-cubic) shows that the splitting field $L$ has Galois group $S_3$. The quadratic extension obtained by adjoining $\sqrt\Delta$ is ramified, so $L/\mathbb Q_3$ is totally ramified. Therefore

$$
G_{-1}=G_0=S_3,
\qquad
G_1=A_3,
$$

because the [wild inertia group](../../../arithmetic.md#wild-inertia-group) is the unique Sylow $3$-subgroup of $S_3$.

It remains to find the wild break. Since

$$
f'(\alpha)=3(\alpha^2+1)
$$

and $\alpha^2+1$ is a unit, the [different ideal](../../../arithmetic.md#different-ideal) of $E/\mathbb Q_3$ has exponent $v_E(f'(\alpha))=3$. The extension $L/E$ is a tamely ramified quadratic extension and has different exponent one. The [different in a tower](../../../arithmetic.md#different-in-a-tower) therefore gives different exponent

$$
d(L/\mathbb Q_3)=1+2\cdot3=7.
$$

On the other hand, the [different exponent from ramification groups](../../../arithmetic.md#different-exponent-from-ramification-groups) is

$$
7=\sum_{i\geq0}(|G_i|-1)
=5+2b,
$$

where $b$ is the last index for which $G_b=A_3$. Thus $b=1$, and

$$
\boxed{G_{-1}=G_0=S_3,\qquad G_1=A_3,\qquad G_i=1\quad(i\geq2).}
$$

## 4

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

[Krasner's lemma](../../../arithmetic.md#krasner-s-lemma) says that if $K$ is complete, $\alpha$ is separable over $K$, and

$$
|\beta-\alpha|<
\min_{\substack{\sigma(\alpha)\ne\alpha\\\sigma\in\operatorname{Gal}(\overline K/K)}}
|\alpha-\sigma(\alpha)|,
$$

then $K(\alpha)\subseteq K(\beta)$.

To prove it, let $\tau$ be an automorphism of $\overline K$ fixing $K(\beta)$. The absolute value has a unique extension to every finite extension of the complete field $K$, so it is invariant under $\tau$. If $\tau(\alpha)\ne\alpha$, the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality) and the displayed strict inequality give

$$
|\tau(\alpha)-\beta|
=|\tau(\alpha)-\alpha|
>|\alpha-\beta|.
$$

But $\tau(\beta)=\beta$ and invariance gives $|\tau(\alpha)-\beta|=|\alpha-\beta|$, a contradiction. Every automorphism fixing $K(\beta)$ therefore fixes $\alpha$, which proves the field inclusion by [Galois correspondence](../../../galois-theory.md#galois-correspondence).

Now let $L/\mathbb Q_p$ be finite. By the [primitive element theorem](../../../galois-theory.md#primitive-element-theorem), write $L=\mathbb Q_p(\alpha)$ with separable minimal polynomial $f\in\mathbb Q_p[X]$. Approximate the coefficients of $f$ closely by those of a polynomial $g\in\mathbb Q[X]$ of the same degree. [Continuity of roots over a non-Archimedean field](../../../arithmetic.md#continuity-of-roots-over-a-non-archimedean-field) gives a root $\beta$ of $g$ arbitrarily close to $\alpha$. Choose it close enough for [Krasner's lemma](../../../arithmetic.md#krasner-s-lemma); then

$$
\mathbb Q_p(\alpha)\subseteq\mathbb Q_p(\beta).
$$

The degree bound from $\deg g=\deg f$ forces equality. If $F=\mathbb Q(\beta)$ and $\mathfrak p$ is the prime selected by the embedding $F\hookrightarrow\overline{\mathbb Q}_p$, its completion is

$$
F_{\mathfrak p}\cong\mathbb Q_p(\beta)=L.
$$

**Thus every finite extension of $\mathbb Q_p$ is the [completion of a number field at a prime ideal](../../../arithmetic.md#completion-of-a-number-field-at-a-prime-ideal).**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $G=\operatorname{Gal}(L/K)$ and let $\mathcal P,\mathcal Q$ lie over $\mathfrak p$. These primes define two extensions to $L$ of the $\mathfrak p$-adic absolute value on $K$. The [conjugacy of extensions of a valuation to a normal extension](../../../arithmetic.md#conjugacy-of-extensions-of-a-valuation-to-a-normal-extension) says that some $\sigma\in G$ carries the first extension to the second. Equivalently, $\sigma\mathcal P=\mathcal Q$. This proves the [transitivity of the Galois action on primes](../../../arithmetic.md#transitivity-of-the-galois-action-on-primes).

The [decomposition group](../../../arithmetic.md#decomposition-group) is the stabilizer

$$
G_{\mathcal P/\mathfrak p}
=\{\sigma\in G:\sigma\mathcal P=\mathcal P\}.
$$

Each such automorphism extends continuously to the completions, and restriction gives the [decomposition group of a prime and local Galois group](../../../arithmetic.md#decomposition-group-of-a-prime-and-local-galois-group) isomorphism

$$
G_{\mathcal P/\mathfrak p}\cong
\operatorname{Gal}(L_{\mathcal P}/K_{\mathfrak p}).
$$

For the splitting field $L=\mathbb Q(\sqrt[3]7,\zeta_3)$ of $X^3-7$, the global Galois group is $S_3$. Since $7\equiv1\pmod3$, the field $\mathbb Q_7$ contains $\zeta_3$. The local splitting field is therefore $\mathbb Q_7(\sqrt[3]7)$, an Eisenstein, totally ramified cyclic extension of degree three. Hence there are

$$
[S_3:C_3]=2
$$

primes of $L$ above $7$, and the decomposition group of each is the normal subgroup

$$
\boxed{A_3\cong C_3.}
$$

## 5

↑ **Parent:** [Paper 136](paper-136.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For the [discrete valuation](../../../commutative-algebra.md#discrete-valuation) $v$ corresponding to $|\mathord\cdot|$, the [valuation ring](../../../commutative-algebra.md#valuation-ring) and its maximal ideal are

$$
\mathcal O_K=\{x\in K:v(x)\geq0\},
\qquad
\mathfrak m=\{x\in K:v(x)>0\}.
$$

The first is a subring of the field $K$, hence an [integral domain](../../../commutative-algebra.md#integral-domain). An element of $\mathcal O_K$ is a unit exactly when its valuation is zero, so every nonunit lies in $\mathfrak m$ and $\mathfrak m$ is the unique [maximal ideal](../../../commutative-algebra.md#maximal-ideal).

Choose a [uniformizer](../../../commutative-algebra.md#uniformizer) $\pi$ with $v(\pi)=1$. If $I\ne0$ is an ideal, the set of valuations of its nonzero elements has a least member $n$. Choose $x\in I$ with $v(x)=n$. Then $x=u\pi^n$ for a unit $u$, so $(x)=(\pi^n)$. Every $y\in I$ has $v(y)\geq n$, hence $y/x\in\mathcal O_K$, and therefore $I=(x)$. Thus $\mathcal O_K$ is a [discrete valuation ring](../../../commutative-algebra.md#discrete-valuation-ring), in particular a [principal ideal domain](../../../commutative-algebra.md#principal-ideal-domain).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

If $K$ is complete and $L/K$ is finite, the [unique extension of an absolute value to a finite extension](../../../arithmetic.md#unique-extension-of-an-absolute-value-to-a-finite-extension) is

$$
|x|_L=|N_{L/K}(x)|^{1/[L:K]}.
$$

It restricts to the given absolute value because $N_{L/K}(a)=a^{[L:K]}$ for $a\in K$. The usual construction through multiplication by $x$ on the finite-dimensional $K$-vector space $L$, together with completeness, proves that this is the only extending absolute value.

For $\sigma\in\operatorname{Gal}(L/K)$, the map $x\mapsto|\sigma(x)|_L$ is another absolute value extending $|\mathord\cdot|$ on $K$. Uniqueness therefore gives

$$
\boxed{|\sigma(x)|_L=|x|_L.}
$$

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Assume first that $K$ is complete. If $x$ is integral over $\mathcal O_K$, its monic equation and the [ultrametric inequality](../../../arithmetic.md#ultrametric-inequality) imply $|x|_L\leq1$, so $x\in\mathcal O_L$. Conversely, if $|x|_L\leq1$, part (i) gives $|\sigma(x)|_L\leq1$ for every $K$-embedding $\sigma$. The coefficients of the minimal polynomial of $x$ are elementary symmetric polynomials in its conjugates, so they all lie in $\mathcal O_K$. Thus $x$ is integral over $\mathcal O_K$, proving the [integral closure in a finite extension of a complete discretely valued field](../../../arithmetic.md#integral-closure-in-a-finite-extension-of-a-complete-discretely-valued-field) identity $\mathcal O_L=\overline{\mathcal O_K}^{\,L}$.

Completeness is necessary. Give $\mathbb Q$ its $5$-adic absolute value, take $L=\mathbb Q(i)$, and choose the extension corresponding to the prime $(2+i)$ above $5$. Then

$$
x=\frac{2+i}{2-i}
$$

has nonnegative valuation at $(2+i)$, so it belongs to the chosen valuation ring $\mathcal O_L$. At the conjugate prime $(2-i)$ it has negative valuation, so it does not lie in the integral closure of $\mathbb Z_{(5)}$ in $\mathbb Q(i)$. Hence the chosen valuation ring can be strictly larger than the integral closure when the base field is not complete.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
