# Paper 31

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper31.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper31.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)

## 1

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $L/K$ be a finite [Galois extension](../../../galois-theory.md#finite-galois-extension) of [number fields](../../../algebraic-number-theory.md#number-field), with [Galois group](../../../galois-theory.md#galois-group) $G$, and let $\mathfrak p$ be a nonzero [prime ideal](../../../commutative-algebra.md#prime-ideal) of $\mathcal O_K$. Write its [prime ideal factorization](../../../algebraic-number-theory.md#prime-ideal-factorization) as

$$
\mathfrak p\mathcal O_L=\prod_{j=1}^g\mathfrak P_j^{e_j},\qquad
f_j=[\mathcal O_L/\mathfrak P_j:\mathcal O_K/\mathfrak p].
$$

The [Galois group](../../../galois-theory.md#galois-group) acts transitively on the primes above $\mathfrak p$. One proof uses the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem). If $\mathfrak Q$ were outside the orbit of $\mathfrak P$, choose an [integral element](../../../commutative-algebra.md#integral-element) $a$ which is zero modulo $\mathfrak Q$ and one modulo every conjugate of $\mathfrak P$. Its [field norm](../../../algebraic-number-theory.md#field-norm) $\prod_{\sigma\in G}\sigma(a)$ belongs to $\mathfrak Q\cap\mathcal O_K=\mathfrak p$, hence to $\mathfrak P$. But each factor is one modulo $\mathfrak P$, a contradiction. Transitivity also makes all $e_j$ equal to a common [ramification index](../../../arithmetic.md#ramification-index) $e$ and all $f_j$ equal to a common [residue degree](../../../arithmetic.md#residue-degree) $f$.

Fix $\mathfrak P$ above $\mathfrak p$. Its [decomposition group](../../../arithmetic.md#decomposition-group) is the stabilizer

$$
D_{\mathfrak P}=\{\sigma\in G:\sigma\mathfrak P=\mathfrak P\}.
$$

The [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) gives $|D_{\mathfrak P}|=|G|/g$. Elements of $D_{\mathfrak P}$ act on the [residue field](../../../commutative-algebra.md#residue-field) $\kappa(\mathfrak P)$ over $\kappa(\mathfrak p)$; the [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) is the [inertia group](../../../arithmetic.md#inertia-group)

$$
I_{\mathfrak P}=\{\sigma\in D_{\mathfrak P}:\sigma(a)\equiv a\pmod{\mathfrak P}\text{ for all }a\in\mathcal O_L\}.
$$

Thus inertia measures the [automorphisms](../../../algebra.md#automorphism) invisible after reduction, whereas decomposition measures all [automorphisms](../../../algebra.md#automorphism) preserving the chosen prime.

The completion $L_{\mathfrak P}/K_{\mathfrak p}$ is a [Galois extension](../../../galois-theory.md#finite-galois-extension) with [group](../../../group.md) $D_{\mathfrak P}$: preservation of $\mathfrak P$ lets an [automorphism](../../../algebra.md#automorphism) extend continuously to the completion, and the local embeddings of this normal extension arise in this way. The [degree of a field extension](../../../algebra.md#degree-of-a-field-extension) formula is $[L_{\mathfrak P}:K_{\mathfrak p}]=ef$. Reduction gives the [exact sequence](../../../homology.md#exact-sequence)

$$
1\longrightarrow I_{\mathfrak P}\longrightarrow D_{\mathfrak P}
\longrightarrow\operatorname{Gal}(\kappa(\mathfrak P)/\kappa(\mathfrak p))
\longrightarrow1.
$$

For [surjectivity](../../../algebra.md#surjective-function), lift a primitive residue-field generator by the [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) to obtain the [maximal unramified subextension of a local field extension](../../../arithmetic.md#maximal-unramified-subextension-of-a-local-field-extension) of $L_{\mathfrak P}/K_{\mathfrak p}$. Its [automorphisms](../../../algebra.md#automorphism) are the residue-field [automorphisms](../../../algebra.md#automorphism). They extend to $L_{\mathfrak P}$ because the latter is normal. Since a finite [residue field](../../../commutative-algebra.md#residue-field) extension has a cyclic [Galois group](../../../galois-theory.md#galois-group) of order $f$, the [exact sequence](../../../homology.md#exact-sequence) yields

$$
\boxed{|D_{\mathfrak P}|=ef,\qquad |I_{\mathfrak P}|=e,\qquad |D_{\mathfrak P}/I_{\mathfrak P}|=f,\qquad [L:K]=gef.}
$$

The [fixed field](../../../galois-theory.md#fixed-field) of local inertia is the [maximal unramified subextension of a local field extension](../../../arithmetic.md#maximal-unramified-subextension-of-a-local-field-extension), and the extension above it is [totally ramified](../../../arithmetic.md#totally-ramified-extension). Primes in the same global orbit have conjugate [decomposition groups](../../../arithmetic.md#decomposition-group) and [inertia groups](../../../arithmetic.md#inertia-group), so the orders do not depend on the chosen prime.

If $e=1$, inertia is trivial and $D_{\mathfrak P}$ is generated by the unique [Frobenius automorphism](../../../arithmetic.md#frobenius-automorphism) acting on residues by $z\mapsto z^{N\mathfrak p}$. Its order is $f$. In a ramified extension this residue action determines only a coset modulo inertia. A prime splits completely exactly when $e=f=1$, equivalently its [decomposition group](../../../arithmetic.md#decomposition-group) is trivial. A [totally ramified](../../../arithmetic.md#totally-ramified-extension) prime has $g=f=1$ and $I_{\mathfrak P}=D_{\mathfrak P}=G$; an unramified prime has $I_{\mathfrak P}=1$. In an [abelian extension](../../../galois-theory.md#abelian-extension), conjugation does nothing, so the associated [groups](../../../group.md) and unramified [Artin symbol](../../../algebraic-number-theory.md#artin-symbol) are independent of the prime above $\mathfrak p$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Use arithmetic [Frobenius automorphisms](../../../arithmetic.md#frobenius-automorphism): residues are raised to the size of the base [residue field](../../../commutative-algebra.md#residue-field). Let $S$ contain the finite primes ramified in the finite [abelian extension](../../../galois-theory.md#abelian-extension) $L/K$. The [Artin map](../../../algebraic-number-theory.md#artin-reciprocity-law) is the [group homomorphism](../../../group-theory.md#group-homomorphism)

$$
\operatorname{Art}_{L/K}:I_K^S\longrightarrow\operatorname{Gal}(L/K),\qquad
\prod_{\mathfrak p\notin S}\mathfrak p^{n_{\mathfrak p}}
\longmapsto\prod_{\mathfrak p\notin S}\operatorname{Frob}_{\mathfrak p}^{n_{\mathfrak p}},
$$

where $I_K^S$ is the [group](../../../group.md) of [fractional ideals](../../../commutative-algebra.md#fractional-ideal) supported outside $S$. The [Artin symbol](../../../algebraic-number-theory.md#artin-symbol) $\operatorname{Frob}_{\mathfrak p}$ is independent of the prime above $\mathfrak p$, since the extension is abelian. [Commutativity](../../../algebra.md#commutativity) makes the displayed extension from [prime ideals](../../../commutative-algebra.md#prime-ideal) well defined. Defining this map does not yet assert the [Artin reciprocity law](../../../algebraic-number-theory.md#artin-reciprocity-law), which describes its congruence [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism).

For an intermediate [field](../../../algebra.md#field) $K\subseteq E\subseteq L$, restriction gives

$$
\boxed{\operatorname{Art}_{L/K}(\mathfrak a)|_E=\operatorname{Art}_{E/K}(\mathfrak a).}
$$

To prove it, start with an unramified prime $\mathfrak p$ and a prime of $L$ above it. Its [Frobenius automorphism](../../../arithmetic.md#frobenius-automorphism) acts on the residue of every [integral element](../../../commutative-algebra.md#integral-element) of $E$ by raising it to $N\mathfrak p$. Its restriction is therefore the [Frobenius automorphism](../../../arithmetic.md#frobenius-automorphism) for $E/K$ at the restricted prime. The identity for all allowed [fractional ideals](../../../commutative-algebra.md#fractional-ideal) follows by the [group homomorphism](../../../group-theory.md#group-homomorphism) property. On [Galois groups](../../../galois-theory.md#galois-group), restriction is the quotient by $\operatorname{Gal}(L/E)$, so passing to a subextension quotients the [Artin map](../../../algebraic-number-theory.md#artin-reciprocity-law) accordingly.

Now let $E/K$ be any finite extension and put $M=LE$. This is the translated extension: $M/E$ is abelian, and restriction identifies $\operatorname{Gal}(M/E)$ with $\operatorname{Gal}(L/(L\cap E))$. A prime $\mathfrak q$ of $E$ above a prime $\mathfrak p\notin S$ is unramified in $M/E$, because forming a [compositum](../../../algebra.md#field-compositum) with $E$ preserves an [unramified extension](../../../arithmetic.md#unramified-extension). Put $r=f(\mathfrak q/\mathfrak p)$. The residue-field sizes satisfy $N\mathfrak q=(N\mathfrak p)^r$. Consequently the restriction to $L$ of Frobenius at $\mathfrak q$ acts on its integral residues by raising them to $(N\mathfrak p)^r$, giving

$$
\operatorname{Frob}_{\mathfrak q}(M/E)|_L
=\operatorname{Frob}_{\mathfrak p}(L/K)^r.
$$

But the [ideal norm](../../../algebraic-number-theory.md#ideal-norm) is $N_{E/K}\mathfrak q=\mathfrak p^r$. Multiplying this prime-by-prime identity proves

$$
\boxed{\operatorname{Art}_{M/E}(\mathfrak a)|_L
=\operatorname{Art}_{L/K}(N_{E/K}\mathfrak a).}
$$

This is [restriction and norm compatibility of the Artin map](../../../algebraic-number-theory.md#restriction-and-norm-compatibility-of-the-artin-map). The [fractional ideal](../../../commutative-algebra.md#fractional-ideal) $\mathfrak a$ must be supported over primes unramified in $L/K$. No assumption that $E/K$ itself is unramified or Galois is needed. With geometric rather than [arithmetic Frobenius](../../../arithmetic.md#frobenius-automorphism), both maps are inverted and the compatibility identities remain unchanged.

## 2

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

A useful strong form of the [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) is the following. Let $F$ be a [complete discretely valued field](../../../commutative-algebra.md#complete-discretely-valued-field), with [valuation ring](../../../commutative-algebra.md#valuation-ring) $\mathcal O$, normalized [valuation](../../../algebra.md#valuation) $v$, and $P\in\mathcal O[T]$. If $a_0\in\mathcal O$ satisfies

$$
v(P(a_0))>2v(P'(a_0)),
$$

then there is a unique root $a\in\mathcal O$ in the ball $v(a-a_0)>v(P'(a_0))$. When $P(a_0)=0$ the assertion is immediate; otherwise the condition includes $P'(a_0)\ne0$.

Here is a proof by [Newton iteration over a valued field](../../../arithmetic.md#newton-iteration-over-a-valued-field). Write $c=v(P'(a_0))$ and $t_0=v(P(a_0))>2c$, and set

$$
a_{j+1}=a_j-\frac{P(a_j)}{P'(a_j)}.
$$

Suppose $v(P'(a_j))=c$ and $t_j=v(P(a_j))>2c$. The correction has [valuation](../../../algebra.md#valuation) $t_j-c>c\geq0$, so $a_{j+1}\in\mathcal O$. [Taylor expansion](../../../calculus.md#taylor-expansion) over $\mathcal O$ cancels the linear term and gives

$$
v(P(a_{j+1}))\geq2(t_j-c),\qquad
v(P'(a_{j+1})-P'(a_j))\geq t_j-c>c.
$$

Thus the derivative still has [valuation](../../../algebra.md#valuation) $c$, and $t_{j+1}-2c\geq2(t_j-2c)$. Unless an exact root is reached earlier, the corrections tend to zero with exponentially increasing [valuations](../../../algebra.md#valuation). [Completeness](../../../topological-analysis.md#completeness) gives $a_j\to a$, and [continuity](../../../calculus.md#continuous-function) gives $P(a)=0$ and $v(a-a_0)=t_0-c>c$. For uniqueness, if $a,b$ are in this ball, [polynomial](../../../polynomial.md) expansion around $a_0$ gives

$$
P(a)-P(b)=(a-b)\bigl(P'(a_0)+R\bigr),\qquad v(R)>c.
$$

The second factor has [valuation](../../../algebra.md#valuation) exactly $c$ and is nonzero, so two roots in the ball must be equal. In particular, a simple residue root lifts uniquely: $v(P(a_0))\geq1$ and $v(P'(a_0))=0$ satisfy the hypothesis.

For the [square-class group of a p-adic field](../../../galois-theory.md#square-class-group-of-a-p-adic-field), write every element as $p^r u$ with $u\in\mathbb Z_p^\times$. Multiplication by a square changes $r$ by an even [integer](../../../number-theory.md#integer), so [valuation](../../../algebra.md#valuation) parity gives one independent factor $C_2$.

For odd $p$, a unit $u$ is a square if and only if its residue is a square in $\mathbb F_p^\times$. Necessity follows by reduction; sufficiency applies the simple-root [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) to $T^2-u$, whose derivative is a unit at a nonzero residue root. The [cyclic group](../../../group.md#cyclic-group) $\mathbb F_p^\times$ has square [subgroup](../../../group.md#subgroup) of index two. If $u_0$ is a unit with nonsquare residue, then

$$
\boxed{\mathbb Q_p^\times/(\mathbb Q_p^\times)^2\cong C_2^2,qquad\text{representatives }1,u_0,p,pu_0\quad(p\ne2).}
$$

For $p=2$, every odd square is one modulo eight. Conversely, if $u\equiv1\pmod8$, take $P(T)=T^2-u$ and $a_0=1$. Then $v_2(P(1))\geq3>2v_2(P'(1))=2$, so the strong [Hensel lemma](../../../arithmetic.md#hensel-s-lemma) gives a [square root](../../../algebra.md#square-root). Thus unit [square classes](../../../galois-theory.md#square-class) are exactly their residues $1,3,5,7$ modulo eight. The classes $-1$ and $5$ generate this [group](../../../group.md) of order four independently, and [valuation](../../../algebra.md#valuation) parity supplies the class $2$. Hence

$$
\boxed{\mathbb Q_2^\times/(\mathbb Q_2^\times)^2\cong C_2^3,qquad\text{generators }-1,5,2,\quad\text{representatives }\pm1,\pm5,\pm2,\pm10.}
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

For $a,b\in\mathbb Q_p^\times$, the [quadratic Hilbert symbol](../../../arithmetic.md#quadratic-hilbert-symbol) $(a,b)_p$ is one if $b$ is a [field norm](../../../algebraic-number-theory.md#field-norm) from $\mathbb Q_p(\sqrt a)$, and minus one otherwise; a square $a$ gives the trivial extension and symbol one. It depends only on the two [square classes](../../../galois-theory.md#square-class). Equivalently, the conic $z^2=ax^2+by^2$ has a nonzero [rational point](../../../algebraic-geometry.md#rational-point) precisely when the symbol is one. Interchanging $a$ and $b$ in the conic gives $(a,b)_p=(b,a)_p$. The [Hilbert norm residue symbol](../../../arithmetic.md#hilbert-norm-residue-symbol) is a [group homomorphism](../../../group-theory.md#group-homomorphism) in each argument; for nonsquare $a$, the [cyclic local norm index](../../../arithmetic.md#cyclic-local-norm-index) makes its [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) a [subgroup](../../../group.md#subgroup) of index two. The resulting pairing on [square classes](../../../galois-theory.md#square-class) is nondegenerate. Also

$$
(a,-a)_p=1,\qquad(a,a)_p=(a,-1)_p,
$$

since $N(\sqrt a)=-a$. In the language of [local class field theory](../../../arithmetic.md#local-class-field-theory), $(a,b)_p=\operatorname{Art}_p(b)(\sqrt a)/\sqrt a$; in the [Brauer group](../../../associative-algebra.md#brauer-group), it records whether the quaternion [cyclic algebra](../../../associative-algebra.md#cyclic-algebra) $(a,b)$ splits. These are compatible norm-obstruction descriptions.

An [unramified extension](../../../arithmetic.md#unramified-extension) of [local fields](../../../arithmetic.md#local-field) of degree two has norm [group](../../../group.md) consisting precisely of elements with even [valuation](../../../algebra.md#valuation). Indeed,

$$
v_K(Nz)=2v_L(z),
$$

and the norms on units are surjective. For the latter assertion, the norm on the finite [residue fields](../../../commutative-algebra.md#residue-field) is surjective. On successive [higher principal-unit groups](../../../arithmetic.md#higher-principal-unit-group), the congruence

$$
N(1+\pi^r t)\equiv1+\pi^r\operatorname{Tr}_{\kappa_L/\kappa_K}(\bar t)\pmod{\pi^{r+1}}
$$

allows one to correct a proposed unit norm one digit at a time: the residue [field trace](../../../algebraic-number-theory.md#field-trace) is surjective, and [completeness](../../../topological-analysis.md#completeness) makes the corrections converge. An unramified quadratic field is unique up to [isomorphism](../../../algebra.md#isomorphism). Therefore, if $d$ is its defining nonsquare class,

$$
\boxed{(d,b)_p=(-1)^{v_p(b)}.}
$$

For odd $p$, choose the nonsquare unit $u_0$ from part (i). The [polynomial](../../../polynomial.md) $T^2-u_0$ has irreducible separable reduction, so it defines the unramified [quadratic extension](../../../algebra.md#quadratic-extension). Thus

$$
\Delta_1=\{1,u_0\},\qquad\Delta_2=\{1,u_0\}.
$$

The trivial class is included in $\Delta_2$, since a degree-one extension is unramified. The two units pair trivially, while $(u_0,p)_p=-1$. Any class outside $\Delta_1$ has odd [valuation](../../../algebra.md#valuation) and consequently pairs nontrivially with $u_0$. This proves directly

$$
\boxed{\Delta_1^\perp=\Delta_2,\qquad\Delta_2^\perp=\Delta_1\quad(p\ne2).}
$$

For $p=2$, the unit [square classes](../../../galois-theory.md#square-class) from part (i) give $\Delta_1=\{1,-1,5,-5\}$. The element $\omega=(1+\sqrt5)/2$ satisfies $T^2-T-1$; its reduction $T^2+T+1$ is irreducible and separable over $\mathbb F_2$. This shows that $\mathbb Q_2(\sqrt5)$ is unramified of degree two, giving

$$
\Delta_1=\{1,-1,5,-5\},\qquad\Delta_2=\{1,5\}.
$$

For a fully explicit pairing check, use the generators $(-1,5,2)$. We have $(-1,5)_2=1$ and $(-1,2)_2=1$, since $5=N(1+2i)$ and $2=N(1+i)$ from $\mathbb Q_2(i)$. But $(-1,-1)_2=-1$: a norm equal to $-1$ would be a sum of two squares. If either summand had negative [valuation](../../../algebra.md#valuation), the sum would have negative [valuation](../../../algebra.md#valuation) (equal negative [valuations](../../../algebra.md#valuation) give [valuation](../../../algebra.md#valuation) $1-2r<0$); if both were integral, their squares could not sum to $-1\equiv3\pmod4$. Finally, the unramified norm criterion gives $(5,2)_2=-1$. The identity $(a,b)_2=(b,a)_2$ and $(a,a)_2=(a,-1)_2$ determine the remaining entries. Writing $(a,b)_2=(-1)^{B(a,b)}$, the exponent [matrix](../../../vector-space.md#matrix) is

$$
B=\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix}
\quad\text{in the basis }(-1,5,2).
$$

For $b=(-1)^s5^t2^r$, annihilating both generators $-1,5$ of $\Delta_1$ requires $s=r=0$, so $b\in\{1,5\}$. Annihilating $5$ alone requires $r=0$, so $b$ is a unit class. Hence

$$
\boxed{\Delta_1^\perp=\Delta_2,\qquad\Delta_2^\perp=\Delta_1\quad(p=2).}
$$

These are the [Hilbert-symbol annihilators of units and unramified square classes](../../../arithmetic.md#hilbert-symbol-annihilators-of-units-and-unramified-square-classes). Annihilators here are taken with respect to this pairing, or equivalently in the [character group of a finite abelian group](../../../group.md#character-group-of-a-finite-abelian-group) after identifying [square classes](../../../galois-theory.md#square-class) with their Hilbert-symbol characters.

## 3

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

We give the detailed norm-index argument for a cyclic extension $L/K$ of [p-adic fields](../../../arithmetic.md#p-adic-field); thus $K$ is a finite extension of $\mathbb Q_p$. Write $G=\langle\sigma\rangle$, $|G|=n$. For an additive $G$-[module](../../../module-theory.md#module-mathematics) $M$, put $D=\sigma-1$ and $N=1+\sigma+\cdots+\sigma^{n-1}$. The two periodic [Tate cohomology of a cyclic group](../../../group-theory.md#tate-cohomology-of-a-cyclic-group) [groups](../../../group.md) and the [Herbrand quotient](../../../group-theory.md#herbrand-quotient) are

$$
\widehat H^0(G,M)=\ker D/NM,\qquad
\widehat H^{-1}(G,M)=\ker N/DM,\qquad
h_G(M)=\frac{|\widehat H^0(G,M)|}{|\widehat H^{-1}(G,M)|},
$$

when these [groups](../../../group.md) are finite. For multiplicative [modules](../../../module-theory.md#module-mathematics), $N$ is the product of conjugates and $D(z)=\sigma(z)/z$.

The periodic complex alternating $D$ and $N$ gives a six-term [exact sequence](../../../homology.md#exact-sequence) for every [short exact sequence](../../../module-theory.md#short-exact-sequence) of [modules](../../../module-theory.md#module-mathematics). Taking the alternating product of the [finite group](../../../group.md#finite-group) orders in that [exact sequence](../../../homology.md#exact-sequence) proves

$$
h_G(M)=h_G(M')h_G(M'')\quad\text{if }0\to M'\to M\to M''\to0.
$$

For a finite [module](../../../module-theory.md#module-mathematics), the counting fibers gives $|NM|=|M|/|\ker N|$ and $|DM|=|M|/|\ker D|$, so the two Tate [groups](../../../group.md) have equal order. This proves the [Herbrand quotient of a finite module](../../../group-theory.md#herbrand-quotient-of-a-finite-module) is one. It follows that replacing a [module](../../../module-theory.md#module-mathematics) by a finite-index submodule does not change its quotient, whenever the [cohomology groups](../../../cohomology.md#cohomology-group) are finite.

Two basic calculations drive the norm computation. For the trivial [module](../../../module-theory.md#module-mathematics) $\mathbb Z$, $D=0$ and $N$ is multiplication by $n$, so $h_G(\mathbb Z)=n$. For a regular lattice $R[G]$, with $R=\mathbb Z_p$, invariants are constant coefficient vectors and every such vector is a norm: put its constant coefficient in just one coordinate before applying $N$. The [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) of $N$ consists of the coefficient vectors of sum zero. Successively taking [partial sums](../../../real-analysis.md#partial-sum) solves the cyclic difference equation $Dx=y$ for every such vector $y$. Thus both Tate [groups](../../../group.md) vanish and $h_G(R[G])=1$. This is [cyclic cohomology of a regular lattice](../../../group-theory.md#cyclic-cohomology-of-a-regular-lattice).

Let $U_L=\mathcal O_L^\times$ and $U_L^r=1+\mathfrak P_L^r$. For sufficiently large $r$, the [p-adic logarithm](../../../arithmetic.md#p-adic-logarithm) and [p-adic exponential](../../../arithmetic.md#p-adic-exponential-function) are inverse $G$-equivariant [isomorphisms](../../../algebra.md#isomorphism)

$$
\log:U_L^r\xrightarrow{\sim}\mathfrak P_L^r.
$$

To make the range explicit, $r>v_L(p)/(p-1)$ suffices: the higher terms in the logarithm and exponential have greater [valuation](../../../algebra.md#valuation) than their leading terms, their series converge there, and the identities $\log(\exp x)=x$ and $\exp(\log(1+x))=1+x$ remain valid. Thus a deep multiplicative [unit group](../../../algebra.md#unit-group) becomes an additive $\mathbb Z_p$-lattice in $L$.

By the [normal basis theorem](../../../galois-theory.md#normal-basis-theorem), $L\cong K[G]$ as a $K[G]$-module. As a $\mathbb Q_p[G]$-module it is therefore $\mathbb Q_p[G]^{[K:\mathbb Q_p]}$. Transport the regular lattice $M_0=\mathbb Z_p[G]^{[K:\mathbb Q_p]}$ into $L$. Both $M_0$ and $\mathfrak P_L^r$ are full $G$-stable $\mathbb Z_p$-lattices, so their intersection has finite index in each. The [exact sequences](../../../homology.md#exact-sequence) with finite quotients show that the Tate [groups](../../../group.md) of $\mathfrak P_L^r$ are finite and that

$$
h_G(U_L^r)=h_G(\mathfrak P_L^r)=h_G(M_0)=1.
$$

Since $U_L/U_L^r$ is finite, the exact-sequence formula for the [Herbrand quotient](../../../group-theory.md#herbrand-quotient) gives $h_G(U_L)=1$. Finally, the [valuation](../../../algebra.md#valuation) sequence

$$
1\longrightarrow U_L\longrightarrow L^\times\xrightarrow{v_L}\mathbb Z\longrightarrow0
$$

has trivial $G$-action on $\mathbb Z$. Hence the [Herbrand quotient of the local multiplicative group](../../../group-theory.md#herbrand-quotient-of-the-local-multiplicative-group) is

$$
h_G(L^\times)=h_G(U_L)h_G(\mathbb Z)=n.
$$

For [completeness](../../../topological-analysis.md#completeness), the denominator vanishes by [Hilbert theorem 90](../../../galois-theory.md#hilbert-s-theorem-90). If $N_{L/K}a=1$, put $c_0=1$ and $c_j=a\sigma(a)\cdots\sigma^{j-1}(a)$. Independence of distinct [field automorphisms](../../../galois-theory.md#field-automorphism) lets us choose $t\in L$ with $b=\sum_{j=0}^{n-1}c_j\sigma^j(t)\ne0$. Since $c_n=1$, shifting the sum gives $\sigma(b)=b/a$. Thus $a=b/\sigma(b)$, a multiplicative coboundary. Therefore $\widehat H^{-1}(G,L^\times)=1$. The invariant [subgroup](../../../group.md#subgroup) of $L^\times$ is $K^\times$, so

$$
\boxed{[K^\times:N_{L/K}L^\times]=[L:K]=n.}
$$

This proves the [cyclic local norm index](../../../arithmetic.md#cyclic-local-norm-index) without assuming local reciprocity. If the extension has [ramification index](../../../arithmetic.md#ramification-index) $e$ and [residue degree](../../../arithmetic.md#residue-degree) $f$, the [valuation](../../../algebra.md#valuation) formula $v_K(Nz)=f\,v_L(z)$ shows that the [valuation](../../../algebra.md#valuation) contribution to the index is $f$. A norm is a unit only when $z$ is a unit, so the remaining contribution is

$$
[U_K:N_{L/K}U_L]=e.
$$

In particular, unit norms are surjective in an unramified cyclic extension. The norm [subgroup](../../../group.md#subgroup) is open: on deep units its logarithm is $\operatorname{Tr}_{L/K}(\mathfrak P_L^r)$, a nonzero full lattice in $K$, and therefore contains a sufficiently deep principal-unit [group](../../../group.md). This connects the index calculation to the open finite-index norm [subgroups](../../../group.md#subgroup) classified by [local class field theory](../../../arithmetic.md#local-class-field-theory).

To finish, the [Hasse norm theorem](../../../algebraic-number-theory.md#hasse-norm-theorem) for a cyclic extension of [number fields](../../../algebraic-number-theory.md#number-field) states that a nonzero element is a global norm if and only if it is a norm at every finite and infinite completion. Here is its Brauer-theoretic proof outline. Associate to $a\in K^\times$ the [cyclic algebra](../../../associative-algebra.md#cyclic-algebra) $A=(L/K,\sigma,a)$, with relations $z\ell=\sigma(\ell)z$ and $z^n=a$. The [splitting criterion for a cyclic algebra](../../../associative-algebra.md#splitting-criterion-for-a-cyclic-algebra) says that it splits exactly when $a=Nc$: if $a=Nc$, multiplication by $L$ and the operator $c\sigma$ realize it as $\operatorname{End}_K(L)$; conversely, in a split [matrix representation](../../../representation-theory.md#matrix-representation), the underlying $n$-dimensional space is one-dimensional over $L$, so $z$ must act as $c\sigma$ and $z^n=Nc$.

Apply this criterion at every completion, using the restricted cyclic character and any one completion of $L$ above that place. If $a$ is a local norm everywhere, every localized Brauer class is zero. [Injectivity](../../../algebra.md#injective-function) in the [Albert-Brauer-Hasse-Noether theorem](../../../associative-algebra.md#albert-brauer-hasse-noether-theorem) forces $[A]=0$ in $\operatorname{Br}(K)$; the global splitting criterion gives $a=Nc$. Conversely, a global norm is a local norm after completion, since the norm on $L\otimes_K K_v$ is the product of the component norms, whose images coincide in the Galois case. **The cyclic hypothesis is essential**; the stated local-global principle does not hold for arbitrary extensions.

## 4

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Brauer group](../../../associative-algebra.md#brauer-group) of a [field](../../../algebra.md#field) consists of [equivalence classes](../../../set-theory.md#equivalence-class) of [central simple algebras](../../../associative-algebra.md#central-simple-algebra), with addition induced by [tensor product](../../../linear-algebra.md#tensor-product), zero represented by [matrix algebras](../../../associative-algebra.md#matrix-algebra), and inverse represented by the [opposite algebra](../../../associative-algebra.md#opposite-algebra). Localization sends a global algebra to its scalar extensions at the completions. For a non-Archimedean completion of a [number field](../../../algebraic-number-theory.md#number-field), the [local Brauer invariant](../../../associative-algebra.md#local-brauer-invariant) is an [isomorphism](../../../algebra.md#isomorphism)

$$
\operatorname{inv}_v:\operatorname{Br}(K_v)\xrightarrow{\sim}\mathbb Q/\mathbb Z.
$$

Normalize it so that an unramified [cyclic algebra](../../../associative-algebra.md#cyclic-algebra) of degree $m$, with [arithmetic Frobenius](../../../arithmetic.md#frobenius-automorphism) generator and parameter $a$, has invariant $v(a)/m$. For a real completion, $\operatorname{Br}(\mathbb R)=\mathbb Z/2$ with the Hamilton [quaternion algebra](../../../associative-algebra.md#quaternion-algebra) mapped to $1/2$; for a complex completion the [Brauer group](../../../associative-algebra.md#brauer-group) is zero.

The global computation is the [exact sequence](../../../homology.md#exact-sequence) in the [Albert-Brauer-Hasse-Noether theorem](../../../associative-algebra.md#albert-brauer-hasse-noether-theorem):

$$
\boxed{0\longrightarrow\operatorname{Br}(K)
\longrightarrow\bigoplus_v\operatorname{Br}(K_v)
\xrightarrow{\sum_v\operatorname{inv}_v}\mathbb Q/\mathbb Z
\longrightarrow0.}
$$

Thus a global Brauer class is determined uniquely by a finite-support family of local invariants. Such a family occurs if and only if its sum is zero; at real places the only allowed entries are $0,1/2$, and at complex places the entry is zero. [Injectivity](../../../algebra.md#injective-function) is a local-global splitting principle; the middle exactness is the reciprocity constraint; [surjectivity](../../../algebra.md#surjective-function) of the sum follows already from any one finite local summand. These are separate assertions, not merely different descriptions of the sum formula.

For an explicit [group](../../../group.md) description, choose one finite place $v_0$. Assign arbitrary finite-support invariants at all other finite places and arbitrary allowed invariants at the real places, then set the invariant at $v_0$ equal to minus their sum. This gives

$$
\operatorname{Br}(K)\cong
\left(\bigoplus_{v\ {
m finite},\ v\ne v_0}\mathbb Q/\mathbb Z\right)
\oplus(\mathbb Z/2)^{r_1}.
$$

The description by the entire invariant family is canonical; this displayed elimination of one coordinate depends on the choice of $v_0$.

The connection with [Artin reciprocity](../../../algebraic-number-theory.md#artin-reciprocity-law) is especially transparent for [cyclic algebras](../../../associative-algebra.md#cyclic-algebra). Let $\chi:\operatorname{Gal}(L/K)\hookrightarrow\mathbb Q/\mathbb Z$ describe a cyclic extension, with $\chi(\sigma)=1/n$. Write $(\chi,a)$ for the class of $(L/K,\sigma,a)$. The local reciprocity pairing is

$$
\operatorname{inv}_v(\chi_v,a_v)
=\chi_v\bigl(\operatorname{Art}_{K_v}(a_v)\bigr).
$$

It follows from the [local fundamental class](../../../associative-algebra.md#local-fundamental-class) construction of the [Local Artin map](../../../arithmetic.md#local-artin-map); on an unramified character it is precisely the normalization $v(a_v)/n$. The [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) in the parameter is the local norm [group](../../../group.md), and restriction/corestriction give the norm compatibility of this pairing.

For a principal parameter $a\in K^\times$, the zero-sum identity for its global [cyclic algebra](../../../associative-algebra.md#cyclic-algebra) therefore reads

$$
\sum_v\chi_v(\operatorname{Art}_{K_v}(a))=0.
$$

On the other hand the idelic [Artin reciprocity law](../../../algebraic-number-theory.md#artin-reciprocity-law) is

$$
\prod_v\operatorname{Art}_{L/K,v}(a)=1
\quad(a\in K^\times),
$$

and evaluating this product by $\chi$ gives exactly that zero-sum identity. Conversely, testing every cyclic character of a finite abelian [Galois group](../../../galois-theory.md#galois-group) separates its elements, so the zero-sum identities for [cyclic algebras](../../../associative-algebra.md#cyclic-algebra) imply this principal-idele reciprocity law for every finite [abelian extension](../../../galois-theory.md#abelian-extension). At almost all places a unit and an unramified character pair trivially, so the sums and products are finite.

The full idelic statement identifies the [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) as $K^\times N_{L/K}J_L$ and induces $J_K/(K^\times N_{L/K}J_L)\cong\operatorname{Gal}(L/K)$. It explains why the local norm-residue pairings must glue globally. The global Brauer theorem supplies, in addition, the [injectivity](../../../algebra.md#injective-function) and realization statements needed to compute all algebra classes; the principal-product identity alone would not prove those statements. For [cyclic algebras](../../../associative-algebra.md#cyclic-algebra) its [injectivity](../../../algebra.md#injective-function) yields the [Hasse norm theorem](../../../algebraic-number-theory.md#hasse-norm-theorem), as in Question 3. In degree two, an invariant is either zero or $1/2$, so the zero-sum law becomes the [Hilbert reciprocity law](../../../arithmetic.md#hilbert-reciprocity-law) $\prod_v(a,b)_v=1$. For example, a [quaternion algebra](../../../associative-algebra.md#quaternion-algebra) over $\mathbb Q$ can be ramified at precisely a prescribed [finite set](../../../set.md#finite-set) of places, including possibly the real place, if and only if that set has even cardinality; the invariants uniquely determine its Brauer class. This illustrates how arithmetic reciprocity becomes a concrete constraint on global algebra structure.

## 5

↑ **Parent:** [Paper 31](paper-31.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

For a [number field](../../../algebraic-number-theory.md#number-field) $K$ and a [modulus of a number field](../../../algebraic-number-theory.md#modulus-of-a-number-field) $\mathfrak m$, let $I_K(\mathfrak m)$ be the [group](../../../group.md) of [fractional ideals](../../../commutative-algebra.md#fractional-ideal) prime to its finite part. Let $P_K(\mathfrak m)$ consist of [principal ideals](../../../commutative-algebra.md#principal-ideal) generated by elements congruent to one modulo its finite part and positive at each real place in its infinite part. The [ray class group](../../../algebraic-number-theory.md#ray-class-group) is $\operatorname{Cl}_{\mathfrak m}(K)=I_K(\mathfrak m)/P_K(\mathfrak m)$.

The classification theorem of [class field theory](../../../algebraic-number-theory.md#class-field-theory) asserts the existence of a [ray class field](../../../algebraic-number-theory.md#ray-class-field) $K_{\mathfrak m}$ and an [Artin map](../../../algebraic-number-theory.md#artin-reciprocity-law) [isomorphism](../../../algebra.md#isomorphism)

$$
\operatorname{Cl}_{\mathfrak m}(K)\xrightarrow{\sim}\operatorname{Gal}(K_{\mathfrak m}/K).
$$

Its [intermediate fields](../../../algebra.md#intermediate-field) correspond contravariantly to [subgroups](../../../group.md#subgroup) of this [ray class group](../../../algebraic-number-theory.md#ray-class-group). Equivalently, for each [congruence subgroup of fractional ideals](../../../algebraic-number-theory.md#congruence-subgroup-of-fractional-ideals) $P_K(\mathfrak m)\subseteq H\subseteq I_K(\mathfrak m)$ there is a unique finite [abelian extension](../../../galois-theory.md#abelian-extension) with Artin [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) $H$ and [group](../../../group.md) $I_K(\mathfrak m)/H$. Every finite [abelian extension](../../../galois-theory.md#abelian-extension) occurs for some modulus. For a fixed modulus, these are exactly the extensions whose conductor divides that modulus; the same field may be presented using larger moduli, with the appropriate pulled-back [group kernel](../../../group-theory.md#kernel-of-a-group-homomorphism).

We quote the conductor facts needed to specialize this classification. The finite conductor exponent is zero exactly at the unramified primes. A real place occurs in the conductor exactly when it becomes complex. Thus conductor one means unramified at every finite prime and split at every real place. With $\mathfrak m=1$ the [ray class group](../../../algebraic-number-theory.md#ray-class-group) is the ordinary [ideal class group](../../../algebraic-number-theory.md#ideal-class-group), so classification gives an extension $H_K/K$ with

$$
\boxed{\operatorname{Gal}(H_K/K)\cong\operatorname{Cl}(K),\qquad[H_K:K]=h_K.}
$$

It is unramified at all finite primes, and its real places split. Conversely, every finite [abelian extension](../../../galois-theory.md#abelian-extension) with those properties has conductor one and lies in $K_1=H_K$. This proves the existence and maximality of the ordinary [Hilbert class field](../../../algebraic-number-theory.md#hilbert-class-field). Its degree is finite by finiteness of the [ideal class group](../../../algebraic-number-theory.md#ideal-class-group). The real-place convention matters: allowing real places to become complex gives the narrow class field instead; for the [imaginary quadratic field](../../../algebraic-number-theory.md#imaginary-quadratic-field) in part (ii) this distinction disappears.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Put $t=\sqrt{-30}$ and $K=\mathbb Q(t)$. The [ring of integers](../../../algebraic-number-theory.md#ring-of-integers) is $\mathbb Z[t]$, and the [fundamental discriminant](../../../algebraic-number-theory.md#fundamental-discriminant) is $D_K=-120$. For a [reduced positive definite binary quadratic form](../../../number-theory.md#reduced-positive-definite-binary-quadratic-form) $(a,b,c)$ of discriminant $-120$, reduction gives

$$
|b|\leq a\leq c,\qquad b^2-4ac=-120,\qquad
1\leq a\leq\sqrt{120/3}<7.
$$

The coefficient $b$ is even; checking $1\leq a\leq6$ and $|b|\leq a$, with the usual nonnegative sign choice at boundary equalities, leaves precisely

$$
(1,0,30),\quad(2,0,15),\quad(3,0,10),\quad(5,0,6).
$$

The correspondence between proper quadratic forms and [ideal classes](../../../algebraic-number-theory.md#ideal-class) therefore gives $h_K=4$. All four classes equal their inverses, since inversion replaces $b$ by $-b$. Hence

$$
\operatorname{Cl}(K)\cong C_2\times C_2.
$$

The three nontrivial classes may be represented by the ramified [prime ideals](../../../commutative-algebra.md#prime-ideal) $\mathfrak p_2=(2,t)$, $\mathfrak p_3=(3,t)$ and $\mathfrak p_5=(5,t)$. They square to [principal ideals](../../../commutative-algebra.md#principal-ideal) and satisfy $\mathfrak p_2\mathfrak p_3\mathfrak p_5=(t)$. None is principal: an integral generator of norm $2$, $3$ or $5$ would require $a^2+30b^2$ to equal that number, which is impossible. The relation then makes the three classes distinct, consistently with the four-form calculation.

Consider

$$
H=\mathbb Q(\sqrt2,\sqrt{-3},\sqrt5).
$$

The three rational [square classes](../../../galois-theory.md#square-class) are independent, so $[H:\mathbb Q]=8$. Their radical product is $\sqrt{-30}$, so $K\subset H$ and $[H:K]=4$; the extension $H/K$ is abelian. To verify that it is unramified, rather than assuming that radical adjunctions are harmless at $2,3,5$, use the [conductor-discriminant formula](../../../algebraic-number-theory.md#conductor-discriminant-formula). The seven quadratic subfields have [fundamental discriminants](../../../algebraic-number-theory.md#fundamental-discriminant)

$$
8,\ -3,\ 5,\ -24,\ 40,\ -15,\ -120.
$$

The formula gives

$$
|D_H|=8\cdot3\cdot5\cdot24\cdot40\cdot15\cdot120=120^4.
$$

The discriminant tower identity now gives

$$
|D_H|=|D_K|^{[H:K]}N_{K/\mathbb Q}(\mathfrak d_{H/K}),\qquad
N_{K/\mathbb Q}(\mathfrak d_{H/K})=1.
$$

Thus the [relative discriminant](../../../algebraic-number-theory.md#relative-discriminant) is the [unit ideal](../../../commutative-algebra.md#unit-ideal) and no finite prime ramifies. The base has no real places, so there is no infinite ramification to check. This unramified abelian degree-four extension has degree $h_K$, and part (i) proves

$$
\boxed{H_K=\mathbb Q(\sqrt2,\sqrt{-3},\sqrt5).}
$$

This is the [Hilbert class field of Q of square root minus thirty](../../../algebraic-number-theory.md#hilbert-class-field-of-q-of-square-root-minus-thirty).

Next translate prime representation into an [ideal class](../../../algebraic-number-theory.md#ideal-class). For $p\nmid30$, we claim

$$
p=2x^2+15y^2\text{ for integers }x,y
\quad\Longleftrightarrow\quad
\text{some prime }\mathfrak P\text{ of norm }p\text{ has }[\mathfrak P]=[\mathfrak p_2].
$$

If a representation exists, $\alpha=2x+yt$ lies in $\mathfrak p_2$ and has $N_{K/\mathbb Q}\alpha=2p$. The [integral ideal](../../../commutative-algebra.md#integral-ideal) $(\alpha)\mathfrak p_2^{-1}$ has norm $p$, so it is a [prime ideal](../../../commutative-algebra.md#prime-ideal) $\mathfrak P$. Its class is $[\mathfrak p_2]^{-1}=[\mathfrak p_2]$. Conversely, if $[\mathfrak P]=[\mathfrak p_2]$, the product $\mathfrak p_2\mathfrak P$ is principal, say $(\alpha)$. Since this [ideal](../../../commutative-algebra.md#ideal) lies in $\mathfrak p_2$, its generator has the form $\alpha=2x+yt$ with [integers](../../../number-theory.md#integer) $x,y$. Taking norms gives $4x^2+30y^2=2p$, proving the reverse implication. This is [prime representation via an ideal class](../../../number-theory.md#prime-representation-via-an-ideal-class), and it proves sufficiency as well as necessity.

Identify the required class in $\operatorname{Gal}(H/K)$ through the [Artin map](../../../algebraic-number-theory.md#artin-reciprocity-law). We can use the explicit representation $17=2+15$: $2+t$ has norm $34$, so the prime above $17$ obtained from $(2+t)\mathfrak p_2^{-1}$ has class $[\mathfrak p_2]$. Its Frobenius in the multiquadratic extension acts on the three radicals with signs

$$
\left(\left(\frac2{17}\right),\left(\frac{-3}{17}\right),\left(\frac5{17}\right)\right)=(1,-1,-1).
$$

Their product is one, so this [automorphism](../../../algebra.md#automorphism) fixes $K$. Because $H/\mathbb Q$ is abelian, for any unramified rational prime $p$ that splits in $K$, the Frobenius at either prime of $K$ of norm $p$ is its rational Frobenius restricted to $H/K$. The Artin [isomorphism](../../../algebra.md#isomorphism) therefore makes the required class condition equivalent to

$$
\left(\frac2p\right)=1,\qquad
\left(\frac{-3}p\right)=-1,\qquad
\left(\frac5p\right)=-1.
$$

Conversely, these signs already imply splitting in $K$, since their product is $(\frac{-30}p)=1$. No extra splitting condition is missing.

The supplementary law for $2$, [quadratic reciprocity](../../../number-theory.md#quadratic-reciprocity) for $-3$ and $5$, and then the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem) turn these sign conditions into

$$
p\equiv1\text{ or }7\pmod8,\qquad
p\equiv2\pmod3,\qquad
p\equiv2\text{ or }3\pmod5.
$$

Their four simultaneous [residue classes](../../../number-theory.md#residue-class) modulo $120$ are $17,23,47,113$. Finally, $2$ is represented by $(x,y)=(\pm1,0)$, whereas $3$ and $5$ cannot be represented: $y\ne0$ gives a value at least $15$, and $y=0$ gives twice a square. We have proved the complete criterion

$$
\boxed{p=2x^2+15y^2\text{ is soluble}\iff
p=2\text{ or }p\equiv17,23,47,113\pmod{120}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
