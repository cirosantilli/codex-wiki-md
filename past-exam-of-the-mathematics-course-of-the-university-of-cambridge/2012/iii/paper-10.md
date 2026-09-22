# Paper 10

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_10.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_10.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use $[m]=\{1,\ldots,m\}$. A [combinatorial line](../../../ramsey-theory.md#combinatorial-line) in $[m]^n$ has one nonempty active set of coordinates, all carrying the same variable letter, with every other coordinate fixed. The [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem) states that **for every finite alphabet size $m$ and number of colours $k$, some $n$ makes every $k$-[finite colouring](../../../ramsey-theory.md#finite-coloring) of $[m]^n$ contain a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line)**.

Here is a complete proof through the [alphabet insensitivity lemma](../../../ramsey-theory.md#alphabet-insensitivity-lemma). A $d$-dimensional [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) is obtained from $d$ pairwise disjoint nonempty coordinate blocks, one independently variable letter on each block, and fixed letters elsewhere. For two distinct letters $a,b$, a colouring restricted to such a [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) is $(a,b)$-insensitive if switching $a$ and $b$ in any of its parameter coordinates leaves the colour unchanged, with all other letters and coordinates arbitrary.

We first prove that any desired dimension $d$ admits such an insensitive [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace), using only the [pigeonhole principle](../../../algebra.md#pigeonhole-principle). Define finite bounds recursively by

$$
I(m,k,0)=0,\qquad N=I(m,k^m,d-1),\qquad L=k^{m^N},\qquad I(m,k,d)=L+N.
$$

Split the ambient coordinates into a prefix of length $L$ and a suffix of length $N$. For $0\leq j\leq L$, let the prefix $p_j$ consist of $j$ copies of $b$ followed by $L-j$ copies of $a$. Give it the entire colour profile

$$
\big(c(p_j u):u\in[m]^N\big).
$$

There are at most $k^{m^N}=L$ such profiles, but $L+1$ prefixes. Hence two prefixes $p_s,p_t$, $s<t$, have the same profile. Replace their differing coordinates $s+1,\ldots,t$ by one variable letter, obtaining a prefix word $v(x)$ with $v(a)=p_s$ and $v(b)=p_t$. Then $c(v(a)u)=c(v(b)u)$ for every suffix $u$.

Colour the suffixes by the vector

$$
c'(u)=\big(c(v(x)u):x\in[m]\big),
$$

which has at most $k^m$ colours. By the dimension-$d-1$ induction hypothesis, there is a $(d-1)$-dimensional suffix [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) on which this vector colouring is $(a,b)$-insensitive. Combining it with the variable block of $v$ gives dimension $d$. Switching the first parameter between $a,b$ preserves colour by the equal prefix profiles; switching any other parameter preserves every entry of $c'$ by induction. This proves the [alphabet insensitivity lemma](../../../ramsey-theory.md#alphabet-insensitivity-lemma), including $d=1$, where the suffix is empty.

Now induct on $m$ to prove the [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem). For $m=1$, any one-variable word gives a one-point [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line). Suppose the theorem holds for $m-1$, and let $d$ be a sufficient dimension for $k$ colours on $[m-1]^d$. The lemma supplies a $d$-dimensional [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) insensitive to $(m-1,m)$. Restrict its parameter colouring to $[m-1]^d$. By the alphabet induction hypothesis it contains a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line). Its $m$th point has the same colour as its $(m-1)$st point: switch the active parameter coordinates from $m-1$ to $m$, one at a time. Therefore the full line over $[m]$ is [monochromatic](../../../ramsey-theory.md#monochromatic-set). Its actual active coordinate set is the nonempty union of the active parameter blocks. This completes both inductions.

To deduce the [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem), choose the dimension $n$ for alphabet size $m$ and pull back a colouring of a sufficiently long integer interval along

$$
\Phi(w_1,\ldots,w_n)=\sum_{j=1}^n w_jm^{j-1}.
$$

All images lie in $[N]$ for $N=m\sum_{j=1}^n m^{j-1}$. A [combinatorial line](../../../ramsey-theory.md#combinatorial-line) with active coordinates $D$ maps to

$$
a+d,\ a+2d,\ldots,a+md,\qquad d=\sum_{j\in D}m^{j-1}>0,
$$

where $a$ is the contribution of the fixed coordinates. Thus **every finite colouring of the positive integers contains [monochromatic](../../../ramsey-theory.md#monochromatic-set) [arithmetic progressions](../../../arithmetic.md#arithmetic-progression) of every finite length**. The argument also provides the finite-interval version. Length one is immediate.

The [Strengthened Van der Waerden theorem](../../../ramsey-theory.md#strengthened-van-der-waerden-theorem) requires the common difference itself to have the progression's colour. We prove a useful stronger, scaled version, the [Brauer progression theorem](../../../ramsey-theory.md#brauer-progression-theorem): for every $k,t,\ell\geq1$, a finite bound $B(k,t,\ell)$ guarantees a [monochromatic](../../../ramsey-theory.md#monochromatic-set) set

$$
\boxed{\{td,a,a+d,\ldots,a+(\ell-1)d\},\qquad a,d>0.}
$$

The desired strengthening is $t=1$. For $\ell=1$ choose $a=t,d=1$; for one colour any interval covering the displayed configuration suffices. For the induction on $k$, assume $M=B(k-1,t,\ell)$ and $\ell\geq2$. Put $L=(\ell-1)M+1$, let $W$ be a [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem) bound for $k$ colours and length $L$, and take $B(k,t,\ell)=tMW$. Inside $[W]$, obtain a one-colour progression $a+j\delta$ for $0\leq j<L$, of colour $c$.

All numbers $tj\delta$, $1\leq j\leq M$, lie in the larger interval because $\delta\leq W$. If one has colour $c$, then the subsequence $a,a+j\delta,\ldots,a+(\ell-1)j\delta$, together with $tj\delta$, is the desired configuration with $d=j\delta$. Otherwise the colouring $j\mapsto c(t\delta j)$ of $[M]$ uses at most $k-1$ colours. Apply the induction hypothesis to obtain a one-colour configuration $\{te,b,b+e,\ldots,b+(\ell-1)e\}$ there. Multiplication by $t\delta$ gives common difference $d=t\delta e$ and distinguished point $td=t^2\delta e$, all of the same original colour. This proves the scaled theorem using only the [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem).

**The fixed-active-size strengthening is false.** It already fails for $m=k=2$. For any proposed positive $n,d$, if $d>n$ there is no eligible line. Otherwise colour a word by

$$
\boxed{c(w)=\left\lfloor\frac{\#\{j:w_j=2\}}d\right\rfloor\pmod2.}
$$

The two points of a line with exactly $d$ active coordinates have counts $q$ and $q+d$ of the letter $2$. Their quotient floors differ by exactly one, so their colours differ. This [fixed-active-size obstruction for combinatorial lines](../../../ramsey-theory.md#fixed-active-size-obstruction-for-combinatorial-lines) is valid for every proposed $n,d$. The colouring may depend on $d$, since the assertion chooses $n,d$ before demanding the conclusion for every colouring.

## 2

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Clear a common denominator first, so that all coefficients are nonzero integers. This changes neither the solutions nor [partition regularity](../../../ramsey-theory.md#partition-regular-matrix). We prove the one-equation criterion directly; no form of [Rado's theorem](../../../ramsey-theory.md#rado-s-theorem) is used as an assumption.

For necessity, choose a [prime number](../../../number-theory.md#prime-number) $p>\sum_i|a_i|$. Colour a positive integer by its first nonzero base-$p$ digit: writing $x=p^{v_p(x)}u$ with $p\nmid u$, use the colour $u\pmod p\in\{1,\ldots,p-1\}$. Suppose the equation has a [monochromatic](../../../ramsey-theory.md#monochromatic-set) solution. Let $v$ be the smallest [P-adic valuation](../../../number-theory.md#p-adic-valuation) of its entries and put $I=\{i:v_p(x_i)=v\}$, a nonempty set. Divide the equation by $p^v$ and reduce modulo $p$. All entries indexed by $I$ contribute the same nonzero digit $u$, and all other terms vanish. Hence

$$
u\sum_{i\in I}a_i\equiv0\pmod p.
$$

It follows that $p$ divides $\sum_{i\in I}a_i$. The absolute value of this sum is less than $p$, so **$\boxed{\sum_{i\in I}a_i=0}$**.

For sufficiency, take a nonempty zero-sum index set $I$ and put $S=\sum_{i\notin I}a_i$. If $S=0$, the full coefficient sum is zero and the constant vector $(1,\ldots,1)$ is already a [monochromatic](../../../ramsey-theory.md#monochromatic-set) solution in every colouring. Otherwise choose $j\in I$, put $t=|a_j|$, and set $b_j=-\operatorname{sgn}(a_j)S$, $b_i=0$ for $i\in I\setminus\{j\}$. Then

$$
\sum_{i\in I}a_ib_i=-tS.
$$

Add the same sufficiently large nonnegative integer $H$ to all the $b_i$, obtaining $c_i=b_i+H\geq0$. The sum is unchanged because $\sum_{i\in I}a_i=0$. Let $K=\max_{i\in I}c_i$.

Apply the scaled [Brauer progression theorem](../../../ramsey-theory.md#brauer-progression-theorem), proved above from the permitted [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem), to obtain one-colour numbers $td$ and $a,a+d,\ldots,a+Kd$. Define

$$
x_i=a+c_i d\quad(i\in I),\qquad x_i=td\quad(i\notin I).
$$

All entries are positive and [monochromatic](../../../ramsey-theory.md#monochromatic-set), and

$$
\sum_i a_ix_i=a\sum_{i\in I}a_i+d\sum_{i\in I}a_ic_i+tdS=0-tSd+tSd=0.
$$

Therefore **the row is [partition regular](../../../ramsey-theory.md#partition-regular-matrix) exactly when some nonempty coefficient subset sums to zero**. Repetition of entries is allowed by the definition of [partition regularity](../../../ramsey-theory.md#partition-regular-matrix).

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

**The two versions of [partition regularity](../../../ramsey-theory.md#partition-regular-matrix) are equivalent.** If the row is [partition regular](../../../ramsey-theory.md#partition-regular-matrix) on all positive integers, pull a colouring of the even positive integers back by $n\mapsto2n$. A [monochromatic](../../../ramsey-theory.md#monochromatic-set) solution $\mathbf y$ for this pulled-back colouring gives the even solution $\mathbf x=2\mathbf y$ in the original colouring, since the equation is homogeneous.

Conversely, restrict any colouring of all positive integers to its even members. A [monochromatic](../../../ramsey-theory.md#monochromatic-set) solution supplied by regularity on the even integers is already a valid solution in the full domain. This argument is an instance of [scaling invariance of homogeneous partition regularity](../../../ramsey-theory.md#scaling-invariance-of-homogeneous-partition-regularity) and does not require a new coefficient criterion.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Again use integer coefficients after clearing denominators and put $S=\sum_i a_i$. If $S=0$, choose any odd positive integer $u$ and take all $x_i=u$. This gives a [monochromatic](../../../ramsey-theory.md#monochromatic-set) solution in any colouring.

For necessity, suppose $S\ne0$ and choose $K$ with $2^K>|S|$. Colour the odd positive integers by their [residue classes](../../../number-theory.md#residue-class) modulo $2^K$. In any [monochromatic](../../../ramsey-theory.md#monochromatic-set) candidate, $x_i\equiv u\pmod{2^K}$ for a common odd $u$. The equation would imply $uS\equiv0\pmod{2^K}$. Since $u$ is [coprime](../../../number-theory.md#coprime-integers) to $2^K$, this forces $2^K\mid S$, impossible for nonzero $S$ with $|S|<2^K$. Thus **$\boxed{\text{regular over odd positive integers}\iff\sum_i a_i=0}$**. This is [one-equation partition regularity over odd integers](../../../ramsey-theory.md#one-equation-partition-regularity-over-odd-integers); its obstruction concerns the full coefficient sum rather than just a zero-sum subset.

## 3

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Take $\mathbb N=\{1,2,\ldots\}$. We first prove the [Ellis–Numakura lemma](../../../algebra.md#ellis-numakura-lemma) in the one-sided continuity convention needed here. Let $S$ be a nonempty compact [Hausdorff space](../../../topology.md#hausdorff-space) with an associative multiplication for which each map $x\mapsto xa$ is continuous. Among its nonempty closed [subsemigroups](../../../algebra.md#subsemigroup), there is an inclusion-minimal one, $M$: a decreasing chain has nonempty intersection by compactness, and that intersection is a closed [subsemigroup](../../../algebra.md#subsemigroup), so [Zorn's lemma](../../../set-theory.md#zorn-s-lemma) applies.

Fix $a\in M$. The set $Ma$ is nonempty and compact, hence closed in the [Hausdorff space](../../../topology.md#hausdorff-space), and is a [subsemigroup](../../../algebra.md#subsemigroup) because

$$
(xa)(ya)=\big(x(ay)\big)a\in Ma.
$$

Minimality gives $Ma=M$. Thus the set $T=\{x\in M:xa=a\}$ is nonempty. It is closed by the stated continuity, and it is a [subsemigroup](../../../algebra.md#subsemigroup), since $(xy)a=x(ya)=xa=a$ for $x,y\in T$. Minimality again gives $T=M$, so $a\in T$ and **$\boxed{a^2=a}$**, giving a [semigroup idempotent](../../../algebra.md#idempotent-element-of-a-semigroup). If one instead uses the opposite one-sided continuity convention, the same proof uses $aM$ and $\{x:ax=a\}$; no joint continuity is required.

Apply this lemma to the [Stone-Čech compactification of the natural numbers](../../../set-theory.md#stone-cech-compactification-of-the-natural-numbers) with its given addition. In the [addition on the Stone-Čech compactification of the natural numbers](../../../set-theory.md#addition-on-the-stone-cech-compactification-of-the-natural-numbers) convention,

$$
A\in p+q\iff\{n:A-n\in q\}\in p,\qquad A-n=\{t\in\mathbb N:n+t\in A\}.
$$

The continuous variable is $p$ when $q$ is fixed. The granted compactness, Hausdorff property and associativity therefore imply **there exists an [idempotent ultrafilter](../../../set-theory.md#idempotent-ultrafilter) $p$ with $p+p=p$**.

On the positive integers such a $p$ is nonprincipal: a [principal ultrafilter](../../../set-theory.md#principal-ultrafilter) at $n$ adds to itself to give the one at $2n$, which is different. Hence every cofinite set belongs to $p$. If zero is included in one's convention for $\mathbb N$, use the same compact [semigroup](../../../algebra.md#semigroup) argument on the closed space of [nonprincipal ultrafilters](../../../set-theory.md#nonprincipal-ultrafilter): it is nonempty by compactness of the infinite discrete set's compactification, and the displayed addition sends two free ultrafilters to a free ultrafilter. This avoids the trivial principal idempotent at zero.

To deduce [Hindman's theorem](../../../ramsey-theory.md#hindman-theorem), let $A$ be the unique colour class belonging to $p$. Define

$$
A^*=A\cap\{n:A-n\in p\}.
$$

Idempotence gives $A^*\in p$. The [idempotent-ultrafilter star-set lemma](../../../set-theory.md#idempotent-ultrafilter-star-set-lemma) also gives $A^*-n\in p$ whenever $n\in A^*$. Here is its proof: $A-n\in p$, and applying idempotence to $A-n$ gives

$$
\{t:(A-n)-t\in p\}=\{t:A-(n+t)\in p\}\in p.
$$

Intersecting this set with $A-n$ produces exactly $A^*-n$.

Choose $x_1\in A^*$. Suppose $x_1<\cdots<x_r$ have been chosen with every nonempty finite sum in $A^*$. The finite intersection

$$
A^*\cap\bigcap_{s\in\operatorname{FS}(x_1,\ldots,x_r)}(A^*-s)\cap\{n:n>x_r\}
$$

belongs to $p$, and is therefore nonempty. Choose $x_{r+1}$ from it. The new sums are $x_{r+1}$ and $s+x_{r+1}$, and they all lie in $A^*$. Induction yields

$$
\boxed{\operatorname{FS}(x_1,x_2,\ldots)=\left\{\sum_{i\in F}x_i:\ \varnothing\ne F\subseteq\mathbb N\text{ finite}\right\}\subseteq A.}
$$

This proves **every finite colouring of the positive integers admits a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [finite-sums set](../../../ramsey-theory.md#finite-sums-set) generated by a strictly increasing infinite sequence**, the required [Hindman theorem](../../../ramsey-theory.md#hindman-theorem).

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

**No.** The ten [residue classes](../../../number-theory.md#residue-class) modulo $10$ form a finite partition, so an [ultrafilter](../../../set-theory.md#ultrafilter) $p$ contains exactly one class $C_r$. The addition formula shows that $p+p$ contains $C_{2r}$: for $n\in C_r$, the translate $C_{2r}-n$ is $C_r$ and belongs to $p$. If $p$ is an [idempotent ultrafilter](../../../set-theory.md#idempotent-ultrafilter), uniqueness of its selected class gives $2r\equiv r\pmod{10}$, hence $r=0$.

Thus **every [idempotent ultrafilter](../../../set-theory.md#idempotent-ultrafilter) contains the multiples of $10$**, and cannot also contain their complement. This is the [zero-residue constraint for idempotent ultrafilters](../../../set-theory.md#zero-residue-constraint-for-idempotent-ultrafilters), valid for every finite modulus.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

**Yes.** Use the sequence $x_j=2\cdot10^{j-1}$, $j\geq1$. Every nonempty finite sum has only digits $0$ and $2$ in decimal notation, with leading digit $2$, so none is a power of $10$, including $10^0=1$.

We still need an [idempotent ultrafilter](../../../set-theory.md#idempotent-ultrafilter) containing these sums; merely exhibiting an infinite set is insufficient. Put

$$
F_r=\operatorname{FS}(x_r,x_{r+1},\ldots),\qquad
K=\bigcap_{r\geq1}\overline{F_r},\qquad
\overline{F_r}=\{p:F_r\in p\}.
$$

The nonempty clopen sets $\overline{F_r}$ are nested, so compactness gives a nonempty compact $K$. This is the [tail finite-sums semigroup](../../../set-theory.md#tail-finite-sums-semigroup). To verify closure under addition, take $p,q\in K$ and fix $r$. For any $s\in F_r$, choose a finite representation of $s$ and then an index $t$ beyond every index in that representation. Disjointness of supports gives $F_t\subseteq F_r-s$, so $F_r-s\in q$. Consequently

$$
\{s:F_r-s\in q\}\supseteq F_r\in p,
$$

and $F_r\in p+q$. This holds for every $r$, proving $p+q\in K$. The [Ellis–Numakura lemma](../../../algebra.md#ellis-numakura-lemma) now supplies an [idempotent ultrafilter](../../../set-theory.md#idempotent-ultrafilter) in $K$. It contains $F_1$, a subset of the non-powers of $10$, so by upward closure it contains **the whole set of non-powers of $10$**.

## 4

↑ **Parent:** [Paper 10](paper-10.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $\Omega=[\mathbb N]^\omega$ for the [space of infinite subsets of the natural numbers](../../../ramsey-theory.md#space-of-infinite-subsets-of-the-natural-numbers), identifying a set with its increasing enumeration. If $s$ is finite and $A$ is infinite with every element of $A$ above $\max s$, set

$$
[s,A]=\{s\cup B:B\in[A]^\omega\}.
$$

For the empty stem there is no lower-bound restriction. These sets form the basis of the [Ellentuck topology](../../../ramsey-theory.md#ellentuck-topology), also called the [star topology](../../../ramsey-theory.md#ellentuck-topology). The stem $s$ is fixed, while the infinite tail may be thinned.

A [completely Ramsey set](../../../ramsey-theory.md#completely-ramsey-set) $E\subseteq\Omega$ is one for which every $[s,A]$ admits an infinite $B\subseteq A$ with $[s,B]\subseteq E$ or $[s,B]\cap E=\varnothing$. This keeps the same stem. A [Ramsey set of infinite subsets](../../../ramsey-theory.md#ramsey-set-of-infinite-subsets) requires that every infinite $A$ admit an infinite $B\subseteq A$ with a homogeneous empty-stem cone $[B]^\omega$. It does not require preserving a nonempty finite stem.

A set is a [star-Baire set](../../../ramsey-theory.md#baire-property-in-the-ellentuck-topology) if it differs from a star-open set by a star-[meagre set](../../../topological-analysis.md#meagre-set), equivalently $E\mathbin\triangle U$ is star-meagre for some star-open $U$. A [nowhere dense set](../../../topological-analysis.md#nowhere-dense-set) has closure with empty interior, and a [meagre set](../../../topological-analysis.md#meagre-set) is a countable union of such sets, with both notions interpreted in the specified topology.

For a non-Ramsey example, put $M=\{2,3,\ldots\}$ and well-order all infinite subsets of $M$ as $(A_\alpha)_{\alpha<\mathfrak c}$, where $\mathfrak c=2^{\aleph_0}$. Recursively choose two fresh points $X_\alpha,Y_\alpha\in[A_\alpha]^\omega$, not used at earlier stages. This is possible because each cone has cardinality $\mathfrak c$ and fewer than $\mathfrak c$ points have been used before any stage. Let

$$
C=\{X_\alpha:\alpha<\mathfrak c\},
$$

keeping all the $Y_\alpha$ outside $C$. Every infinite-subset cone on $M$ meets both $C$ and its complement. Thus **$C$ is not Ramsey**, even when regarded as a subset of $\Omega$: any infinite set can first be thinned to avoid $1$. This uses the [axiom of choice](../../../set-theory.md#axiom-of-choice), rather than claiming a Borel counterexample.

Now set

$$
\boxed{E=\{\{1\}\cup X:X\in C\}.}
$$

Every infinite $A$ has an infinite subset $B$ avoiding $1$, and then $[B]^\omega\cap E=\varnothing$. Hence **$E$ is Ramsey**. But no stem-preserving thinning of $[\{1\},M]$ is homogeneous for $E$, because $C$ splits every tail cone. Hence **$E$ is not completely Ramsey**.

To prove the topological equivalence, we first establish the [Ellentuck meagre-set fusion lemma](../../../ramsey-theory.md#ellentuck-meagre-set-fusion-lemma): every star-meagre set can be avoided in a refinement $[s,B]$ with the original stem. Call a set [completely Ramsey-null](../../../ramsey-theory.md#completely-ramsey-null-set) if this avoidance holds in every $[s,A]$.

If $N$ is star-[nowhere dense](../../../topological-analysis.md#nowhere-dense-set), then $U=\Omega\setminus\overline N$ is star-open and dense. By the granted complete-Ramsey property of star-open sets, every $[s,A]$ has a refinement $[s,B]$ either contained in $U$ or disjoint from $U$. The latter alternative would put a nonempty open set inside $\overline N$, contradicting density of $U$. Thus $N$ is [completely Ramsey-null](../../../ramsey-theory.md#completely-ramsey-null-set).

For a countable union $\bigcup_j N_j$ of [completely Ramsey-null](../../../ramsey-theory.md#completely-ramsey-null-set) sets, use fusion, taking care of every possible finite stem. Starting with $A_0=A$, at stage $j$ choose $b_j\in A_{j-1}$ above all previous choices. From the part of $A_{j-1}$ above $b_j$, successively thin an infinite tail for each of the finitely many subsets $t\subseteq\{b_1,\ldots,b_j\}$ so that

$$
[s\cup t,A_j]\cap N_j=\varnothing.
$$

Each thinning keeps the stem $s\cup t$ fixed; subsequent thinnings preserve earlier avoidance. Let $B=\{b_1,b_2,\ldots\}$. For any $X\in[s,B]$ and fixed $j$, put $t=(X\setminus s)\cap\{b_1,\ldots,b_j\}$. The rest of $X$ lies in $A_j$, because all later selected points do. Therefore $X\in[s\cup t,A_j]$ and $X\notin N_j$. Since $j$ was arbitrary,

$$
\boxed{[s,B]\cap\bigcup_jN_j=\varnothing.}
$$

This proves the fusion lemma. Considering all subsets $t$, not merely the single selected prefix, is essential: elements of $[s,B]$ need not use every $b_i$.

Suppose first that $E$ is star-Baire, with $E\triangle U$ star-meagre and $U$ star-open. Thin $[s,A]$ to $[s,B]$ avoiding the meagre difference by the lemma. Then apply the granted complete-Ramsey property of $U$ to find $[s,D]$ homogeneous for $U$, with $D\subseteq B$. On this refinement $E$ and $U$ agree, so it is homogeneous for $E$. Thus $E$ is completely Ramsey.

Conversely, let $E$ be completely Ramsey and let $U$ be the union of all basic neighborhoods wholly contained in $E$, namely its star-interior. Every $[s,A]$ has a homogeneous refinement. If that refinement lies in $E$, it lies in $U$; if it avoids $E$, it also avoids $E\setminus U$. Consequently every basic neighborhood contains a nonempty open refinement disjoint from $E\setminus U$. Since such a refinement is also disjoint from the closure of $E\setminus U$, this difference is star-[nowhere dense](../../../topological-analysis.md#nowhere-dense-set). Thus $E\triangle U=E\setminus U$ is star-meagre, and $E$ is star-Baire. We have proved

$$
\boxed{E\text{ completely Ramsey}\iff E\text{ has the Baire property in the star topology}.}
$$

Finally, **$\Omega$ is not star-meagre**: otherwise apply the fusion lemma to its purported meagre cover inside any nonempty basic neighborhood, obtaining a nonempty $[s,B]$ disjoint from $\Omega$, a contradiction.

The printed paper does not define $\tau$. In the coarser [Ramsey cone topology](../../../ramsey-theory.md#ramsey-cone-topology), whose basic open sets are $[A]^\omega$ without finite stems, **$\Omega$ is $\tau$-meagre**. To prove this, let $D_j=\{X:\min X=j\}$. Its cone-topology closure is $H_j=\{X:j\in X\}$: every cone neighborhood of a point containing $j$ has a subset with least element $j$, whereas if $j\notin X$ the neighborhood $[X]^\omega$ avoids $D_j$. No nonempty cone lies in $H_j$, since its infinite ground set can be thinned to remove $j$. Therefore each $D_j$ is [nowhere dense](../../../topological-analysis.md#nowhere-dense-set), but $\Omega=\bigcup_{j\geq1}D_j$. This proves [meagreness of the Ramsey cone topology](../../../ramsey-theory.md#meagreness-of-the-ramsey-cone-topology) and exhibits the contrast with the [star topology](../../../ramsey-theory.md#ellentuck-topology).

If $\tau$ instead denotes the [ordinary topology on infinite subsets](../../../ramsey-theory.md#ordinary-topology-on-infinite-subsets), with basic cylinders $[s]=\{X:s\text{ is an initial segment of }X\}$, the answer is **not $\tau$-meagre**. Indeed, given countably many nowhere dense sets, extend a finite increasing prefix successively so that its cylinder avoids the closure of the next set. Make the prefix longer at each step. Their union is an infinite increasing enumeration belonging to every chosen cylinder and avoiding the whole proposed cover. The same construction starts inside any nonempty cylinder, so this alternative product topology is also a [Baire space](../../../topological-analysis.md#baire-space). The two conventions have different answers, so the distinction must be made explicitly rather than inferred from the symbol alone.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
