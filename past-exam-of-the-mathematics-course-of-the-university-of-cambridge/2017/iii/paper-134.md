# Paper 134

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_134.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_134.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [a](#1/iii/a)
      - [Solution](#1/iii/a/solution)
    - [b](#1/iii/b)
      - [Solution](#1/iii/b/solution)
    - [c](#1/iii/c)
      - [Solution](#1/iii/c/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [a](#2/iv/a)
      - [Solution](#2/iv/a/solution)
    - [b](#2/iv/b)
      - [Solution](#2/iv/b/solution)
    - [c](#2/iv/c)
      - [Solution](#2/iv/c/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [a](#3/iii/a)
      - [Solution](#3/iii/a/solution)
    - [b](#3/iii/b)
      - [Solution](#3/iii/b/solution)
    - [c](#3/iii/c)
      - [Solution](#3/iii/c/solution)
    - [d](#3/iii/d)
      - [Solution](#3/iii/d/solution)

## 1

↑ **Parent:** [Paper 134](paper-134.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [Nakai–Moishezon criterion](../../../cartier-divisor.md#nakai-moishezon-criterion) says that a [Cartier divisor](../../../cartier-divisor.md) $D$ on a [projective scheme](../../../ringed-space.md#projective-scheme) is [ample](../../../ringed-space.md#ample-line-bundle) exactly when

$$
\boxed{D^{\dim V}\cdot[V]>0\quad\text{for every positive-dimensional integral closed subvariety }V.}
$$

In particular the test includes each positive-dimensional irreducible component. Here and below, “proper” means proper over the ground [field](../../../algebra.md#field), not necessarily a strict subset of $X$. Interpreting it as a strict subset would make the later criteria false even for an integral [projective curve](../../../projective-space.md#projective-curve), whose strict closed [subvarieties](../../../algebraic-geometry.md#closed-subvariety) have dimension zero.

The [intersection product](../../../algebraic-geometry.md#intersection-product-of-cartier-divisors) of [Cartier divisors](../../../cartier-divisor.md) with cycles depends only on their [numerical equivalence of divisors](../../../cartier-divisor.md#numerical-equivalence-of-divisors) classes. One way to see this is to intersect all but one factor first, obtaining a one-cycle; replacing the remaining factor by a numerically equivalent divisor does not change its pairing with that cycle. Multilinearity then handles replacement of every factor. Consequently $D\equiv D'$ makes all the displayed numbers equal. Thus

$$
\boxed{D\equiv D'\Longrightarrow(D\text{ ample}\iff D'\text{ ample}).}
$$

The criterion applies to the integral reduced [subvarieties](../../../algebraic-geometry.md#closed-subvariety) of a possibly [nonreduced scheme](../../../ringed-space.md#nonreduced-scheme); [ampleness on reduced components](../../../ringed-space.md#ampleness-on-reduced-components) explains why the nilpotent structure does not change this condition.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Put $L=\mathcal O_X(D)$ and let $s_D$ be the canonical [global section](../../../ringed-space.md#global-section) cutting out the [effective Cartier divisor](../../../cartier-divisor.md#effective-cartier-divisor) $D$. The [divisor restriction exact sequence](../../../cartier-divisor.md#divisor-restriction-exact-sequence) gives

$$
0\longrightarrow L^{m-1}\xrightarrow{s_D}L^m\longrightarrow L^m|_D\longrightarrow0.
$$

The hypothesis says $L|_D$ is an [ample line bundle](../../../ringed-space.md#ample-line-bundle). By [Serre vanishing](../../../ringed-space.md#serre-vanishing), $H^1(D,L^m|_D)=0$ for all sufficiently large $m$, so the [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) makes

$$
H^1(X,L^{m-1})\longrightarrow H^1(X,L^m)
$$

surjective for all such $m$. These are finite-dimensional [vector spaces](../../../vector-space.md). Their dimensions form a nonincreasing sequence of nonnegative [integers](../../../number-theory.md#integer), so the maps are isomorphisms from some point on. Exactness then implies that the restriction

$$
H^0(X,L^m)\longrightarrow H^0(D,L^m|_D)
$$

is surjective for all sufficiently large $m$.

Choose such an $m$ for which $L^m|_D$ is also a [globally generated line bundle](../../../ringed-space.md#globally-generated-line-bundle). Lift a generating collection of its [global sections](../../../ringed-space.md#global-section) to $X$. At each point of $D$, one lift has nonzero image in the one-dimensional residue-field fibre, hence generates the stalk of $L^m$ by [Nakayama lemma](../../../mathematics.md#nakayama-lemma). Outside $D$, $s_D^m$ is nowhere zero and generates $L^m$. Together these sections generate it everywhere. Therefore

$$
\boxed{\mathcal O_X(mD)\text{ is globally generated for }m\gg0;\quad D\text{ is semiample}.}
$$

This proof works on an arbitrary [projective scheme](../../../ringed-space.md#projective-scheme) because the defining section of an [effective Cartier divisor](../../../cartier-divisor.md#effective-cartier-divisor) is a [non-zero-divisor](../../../mathematics.md#non-zero-divisor). If $D$ is empty, $L\cong\mathcal O_X$ and the conclusion is immediate. [Semiampleness](../../../cartier-divisor.md#semiample-divisor) is the conclusion: the pullback of a line avoiding the centre of a [blowup of a smooth algebraic surface](../../../algebraic-geometry.md#blowup-of-a-smooth-algebraic-surface) of $\mathbb P^2$ satisfies the hypothesis on its support but has zero intersection with the exceptional curve, and therefore is not [ample](../../../ringed-space.md#ample-line-bundle).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/a">a</h4>

↑ **Parent:** [Iii](#1/iii)

<h5 id="1/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#1/iii/a)

Assume $D$ is [ample](../../../ringed-space.md#ample-line-bundle). For every positive-dimensional integral [subvariety](../../../algebraic-geometry.md#closed-subvariety) $V$, its restriction is an [ample Cartier divisor](../../../cartier-divisor.md#ample-cartier-divisor). The [asymptotic Riemann–Roch](../../../ringed-space.md#asymptotic-riemann-roch) polynomial has leading term

$$
\chi(V,\mathcal O_V(mD))=\frac{D^d\cdot[V]}{d!}m^d+O(m^{d-1}),\qquad d=\dim V.
$$

By the [Nakai–Moishezon criterion](../../../cartier-divisor.md#nakai-moishezon-criterion), the coefficient is positive, so this proves implication (a)$\Rightarrow$(b).

For (a)$\Rightarrow$(c), choose $m>0$ such that $\mathcal O_V(mD)$ is [very ample](../../../ringed-space.md#very-ample-line-bundle). Fix a closed point $p\in V$. A hyperplane through its image which does not contain the whole embedded $V$ gives a nonzero [global section](../../../ringed-space.md#global-section) vanishing at $p$. Such a hyperplane exists since $\dim V>0$. Its vanishing is therefore nonempty but not all of $V$. This proves both required forward implications:

$$
\boxed{\text{(a)}\Longrightarrow\text{(b) and (c)}.}
$$

The proofs in the next two sections establish the converse implications. Reduction to integral components is legitimate by [ampleness on reduced components](../../../ringed-space.md#ampleness-on-reduced-components); in dimension zero every [line bundle](../../../ringed-space.md#line-bundle) on a [projective scheme](../../../ringed-space.md#projective-scheme) is [ample](../../../ringed-space.md#ample-line-bundle) and there is no positive-dimensional [subvariety](../../../algebraic-geometry.md#closed-subvariety) to test.

<h4 id="1/iii/b">b</h4>

↑ **Parent:** [Iii](#1/iii)

<h5 id="1/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#1/iii/b)

We prove (b)$\Rightarrow$(a) by induction on dimension, using the independently proved (c)$\Rightarrow$(a) argument in the next section. Work on an integral [projective variety](../../../projective-space.md#projective-variety) $V$ of dimension $d>0$. The hypothesis is inherited by all its integral closed [subvarieties](../../../algebraic-geometry.md#closed-subvariety). Induction therefore makes $D$ [ample](../../../ringed-space.md#ample-line-bundle) on every strictly lower-dimensional closed reduced [subvariety](../../../algebraic-geometry.md#closed-subvariety), and hence on every proper closed subscheme of dimension less than $d$, by [ampleness on reduced components](../../../ringed-space.md#ampleness-on-reduced-components).

Choose an [effective Cartier divisor](../../../cartier-divisor.md#effective-cartier-divisor) $H$ which is a [very ample](../../../ringed-space.md#very-ample-line-bundle) hyperplane section of $V$. Then $\mathcal O_H(D)$ is [ample](../../../ringed-space.md#ample-line-bundle). We need a vanishing statement uniform in extra positive $H$-twists:

$$
H^j(H,\mathcal O_H(mD+tH))=0\qquad(j>0,\ m\ge M,\ t\ge0).
$$

Here is a justification using [Castelnuovo–Mumford regularity](../../../ringed-space.md#castelnuovo-mumford-regularity). Embed $H$ by $\mathcal O_H(H)$. For each of the finitely many positive cohomology degrees $j$, [Serre vanishing](../../../ringed-space.md#serre-vanishing) for the [ample](../../../ringed-space.md#ample-line-bundle) bundle $\mathcal O_H(D)$ makes $H^j(H,\mathcal O_H(mD-jH))$ vanish for $m\ge M$. Thus the pushed-forward sheaf $\mathcal O_H(mD)$ is zero-regular. Persistence of regularity makes it $t+j$-regular for every $t\ge0$, giving exactly the displayed vanishing. This is the [uniform Serre vanishing for two ample twists](../../../ringed-space.md#uniform-serre-vanishing-for-two-ample-twists) lemma. It does not assume that $D$ is [ample](../../../ringed-space.md#ample-line-bundle) on $V$.

Apply the [divisor restriction exact sequence](../../../cartier-divisor.md#divisor-restriction-exact-sequence) to $H$ with twists $mD+tH$. For $i\ge2$, both neighbouring cohomology groups on $H$ vanish, so

$$
H^i(V,\mathcal O_V(mD+tH))\cong H^i(V,\mathcal O_V(mD+(t+1)H))\qquad(t\ge0).
$$

For a fixed $m\ge M$, sufficiently large $t$ kills the right-hand cohomology by [Serre vanishing](../../../ringed-space.md#serre-vanishing) for $H$ on $V$. The [higher cohomology vanishing from an ample hyperplane restriction](../../../ringed-space.md#higher-cohomology-vanishing-from-an-ample-hyperplane-restriction) argument gives $H^i(V,\mathcal O_V(mD))=0$ for all $i\ge2$. Consequently

$$
h^0(V,mD)=\chi(V,mD)+h^1(V,mD)\ge\chi(V,mD)\longrightarrow\infty.
$$

This step is essential: divergence of a polynomial does not by itself prove that its top-degree coefficient is positive.

For $m$ large enough, $h^0(V,mD)>1$. Evaluation at a closed point has a one-dimensional target, so its kernel contains a nonzero section vanishing there. We have obtained condition (c) on $V$. Lower-dimensional [subvarieties](../../../algebraic-geometry.md#closed-subvariety) already have the same property by induction, so the next section's implication (c)$\Rightarrow$(a) applies. Thus

$$
\boxed{\text{(b)}\Longrightarrow\text{(a)}}.
$$

For $d=1$, higher groups with $i\ge2$ vanish automatically and the same evaluation argument starts the induction. The regularity facts used above are stated in [the Stacks Project, regularity lemmas](https://stacks.math.columbia.edu/tag/08A2).

<h4 id="1/iii/c">c</h4>

↑ **Parent:** [Iii](#1/iii)

<h5 id="1/iii/c/solution">Solution</h5>

↑ **Parent:** [C](#1/iii/c)

We prove (c)$\Rightarrow$(a) by induction on dimension. It suffices to work on an integral [projective variety](../../../projective-space.md#projective-variety) $V$. By induction, $D$ is [ample](../../../ringed-space.md#ample-line-bundle) on every lower-dimensional integral [subvariety](../../../algebraic-geometry.md#closed-subvariety), and hence on every lower-dimensional closed subscheme by [ampleness on reduced components](../../../ringed-space.md#ampleness-on-reduced-components).

Apply (c) to $V$ itself. The nonzero section of $\mathcal O_V(mD)$ has a nonempty zero divisor $E$. Because $V$ is integral, this is an [effective Cartier divisor](../../../cartier-divisor.md#effective-cartier-divisor) and $\mathcal O_V(E)\cong\mathcal O_V(mD)$. Its support has dimension less than $\dim V$, so $D|_E$, and therefore $\mathcal O_E(E)$, is [ample](../../../ringed-space.md#ample-line-bundle). Part (ii) makes $E$ [semiample](../../../cartier-divisor.md#semiample-divisor), hence some positive multiple of $D$ is [basepoint-free](../../../cartier-divisor.md#basepoint-free-divisor).

Let $f:V\to Y\subset\mathbb P^N$ be the resulting [Kodaira map](../../../ringed-space.md#kodaira-map), with $\mathcal O_V(qD)=f^*\mathcal O_Y(1)$. No fibre can have positive dimension: such a projective fibre contains an integral [projective curve](../../../projective-space.md#projective-curve) $C$, on which $D$ has degree zero. But the assumed nonzero section of some $\mathcal O_C(rD)$ cannot vanish anywhere, since its nonempty [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) would have positive degree. This contradicts (c).

Thus $f$ has zero-dimensional fibres. A proper [quasi-finite morphism](../../../ringed-space.md#quasi-finite-morphism) is a [finite morphism](../../../algebraic-geometry.md#finite-morphism). The [finite pullback of an ample line bundle](../../../ringed-space.md#finite-pullback-of-an-ample-line-bundle) is [ample](../../../ringed-space.md#ample-line-bundle), so $qD$ and then $D$ are [ample](../../../ringed-space.md#ample-line-bundle). This proves

$$
\boxed{\text{(c)}\Longrightarrow\text{(a)};\qquad\text{(a), (b), (c) are equivalent}.}
$$

The fibre argument proves the [semiample and curve-positive ampleness criterion](../../../cartier-divisor.md#semiample-and-curve-positive-ampleness-criterion). It also explains why testing only existence of a nonzero section, without requiring a zero, would be insufficient: the trivial bundle on a positive-dimensional [projective variety](../../../projective-space.md#projective-variety) has a nowhere-vanishing section.

## 2

↑ **Parent:** [Paper 134](paper-134.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

On a [smooth algebraic surface](../../../algebraic-geometry.md#smooth-algebraic-surface), distinct integral curves have nonnegative [intersection numbers](../../../algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve), because their [intersection multiplicities](../../../algebraic-geometry.md#intersection-multiplicity) are nonnegative. For any member $E\in|D|$ of the [complete linear system of a divisor](../../../cartier-divisor.md#complete-linear-system-of-a-divisor), $E\cdot C=D\cdot C<0$. Hence $C$ must be a component of $E$; otherwise the intersection would be nonnegative.

Subtracting one copy of $C$ from every effective member gives precisely the effective members linearly equivalent to $D-C$. Conversely adding $C$ gives a member of $|D|$. Thus $C$ is a [fixed component](../../../cartier-divisor.md#fixed-component) and

$$
\boxed{|D|=|D-C|+C.}
$$

Equivalently, multiplication by its defining section induces an isomorphism $H^0(X,\mathcal O_X(D-C))\xrightarrow{\sim}H^0(X,\mathcal O_X(D))$. The original PDF has this linear-system equality; the TeX loses the bars and reduces it to an uninformative divisor identity.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Part (i) first shows that $D-C$ is effective. Also $C^2<0$: writing $D=aC+E$ with $a\ge1$ and $E$ effective without $C$ as a component gives $D\cdot C=aC^2+E\cdot C$, where $E\cdot C\ge0$.

For $0\le j<m$,

$$
(mD-jC)\cdot C=m(D-C)\cdot C+(m-j)C^2<0.
$$

Every effective member of $|mD|$ therefore contains $C$; after subtracting it, the same reasoning applies again, until $m$ copies have been subtracted. Conversely adding $mC$ to an effective member of $|m(D-C)|$ is allowed. Hence

$$
\boxed{|mD|=|m(D-C)|+mC\qquad(m\ge0).}
$$

For $m=0$ this is just the identity system $|0|$. The extra intersection hypothesis is needed: on the [Hirzebruch surface](../../../toric-geometry.md#hirzebruch-surface) $\mathbb F_2$, with negative section $S$ and fibre $F$, take $D=S+F$. Then $D\cdot S=-1$ but $(D-S)\cdot S=1$. Here $h^0(2D)=4$ while $h^0(2F)=3$, so removing $2S$ loses a section.

For the point [blowup of a smooth algebraic surface](../../../algebraic-geometry.md#blowup-of-a-smooth-algebraic-surface) $\psi:\widetilde X\to X$ with exceptional curve $E$, the [canonical divisor formula for a surface blowup](../../../algebraic-geometry.md#canonical-divisor-formula-for-a-surface-blowup) and the [intersection formula for blowing up a surface](../../../algebraic-geometry.md#intersection-formula-for-blowing-up-a-surface) give

$$
K_{\widetilde X}=\psi^*K_X+E,\qquad E^2=-1,\qquad\psi^*K_X\cdot E=0.
$$

One must not assume $K_{\widetilde X}$ itself is effective. Instead, if an effective member of $|mK_{\widetilde X}|$ exists, then for each $0\le j<m$ its class after removing $jE$ has intersection $-m+j<0$ with $E$. The same fixed-component argument removes exactly the required $mE$, giving

$$
H^0(\widetilde X,\mathcal O(m\psi^*K_X))\xrightarrow{\ \cdot s_E^m\ }H^0(\widetilde X,\mathcal O(mK_{\widetilde X}))
$$

as an isomorphism, also when both sides are zero. Since $X$ is normal and $\psi$ is proper and birational, $\psi_*\mathcal O_{\widetilde X}=\mathcal O_X$. The [projection formula for sheaves](../../../ringed-space.md#projection-formula) therefore identifies the space on the left with $H^0(X,\mathcal O_X(mK_X))$. Consequently

$$
\boxed{H^0(\widetilde X,mK_{\widetilde X})\cong H^0(X,mK_X)\quad(m\ge0).}
$$

The PDF writes equality of spaces; this is the canonical identification just described, rather than literal equality of spaces on different schemes. This proves [blowup invariance of plurigenera](../../../ringed-space.md#blowup-invariance-of-plurigenera) in arbitrary characteristic.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Because $C\cong\mathbb P^1$ and $\deg\mathcal O_C(C)=C^2=0$, its normal [line bundle](../../../ringed-space.md#line-bundle) is $\mathcal O_C(C)\cong\mathcal O_{\mathbb P^1}$. Thus every $\mathcal O_C(mC)$ is trivial and has $H^1=0$. The [divisor restriction exact sequence](../../../cartier-divisor.md#divisor-restriction-exact-sequence) gives, for every $m\ge1$,

$$
0\to\mathcal O_X((m-1)C)\to\mathcal O_X(mC)\to\mathcal O_C\to0.
$$

The maps $H^1(X,(m-1)C)\to H^1(X,mC)$ are surjective. Their nonnegative finite dimensions eventually stabilize, so for every sufficiently large $m$ restriction $H^0(X,mC)\to H^0(C,\mathcal O_C)=k$ is surjective. A lift of $1$ is nowhere zero along $C$, and the canonical section of $mC$ is nowhere zero outside $C$. Together they generate $\mathcal O_X(mC)$. Therefore $C$ is [semiample](../../../cartier-divisor.md#semiample-divisor).

For those same large $m$, the exact sequence of [global sections](../../../ringed-space.md#global-section) gives

$$
h^0(X,mC)-h^0(X,(m-1)C)=1.
$$

Thus $h^0(X,mC)=m+O(1)$, and the [Iitaka dimension](../../../cartier-divisor.md#iitaka-dimension) is exactly one:

$$
\boxed{C\text{ is semiample},\qquad\kappa(C)=1.}
$$

Equivalently, its basepoint-free multiple defines a morphism to a curve: it is nonconstant because its sections grow, and cannot have two-dimensional image because $(mC)^2=0$. This is the [semiampleness of a square-zero rational curve](../../../cartier-divisor.md#semiampleness-of-a-square-zero-rational-curve); it uses no characteristic-zero vanishing theorem.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/a">a</h4>

↑ **Parent:** [Iv](#2/iv)

<h5 id="2/iv/a/solution">Solution</h5>

↑ **Parent:** [A](#2/iv/a)

By [Kodaira's lemma](../../../cartier-divisor.md#kodaira-s-lemma) for the [big divisor](../../../cartier-divisor.md#big-divisor) $K_X$, choose an integer $q>0$, an [ample Cartier divisor](../../../cartier-divisor.md#ample-cartier-divisor) $A$, and an [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) $E$ with

$$
qK_X\sim A+E.
$$

If an integral curve $C$ is not a component of $E$, nonnegative intersections of distinct curves give

$$
qK_X\cdot C=A\cdot C+E\cdot C>0.
$$

Thus every curve with $K_X\cdot C<0$ is one of the finitely many components of $E$. In particular,

$$
\boxed{\operatorname{Neg}(K_X)\subseteq\operatorname{Supp}_{\mathrm{components}}(E),\quad\operatorname{Neg}(K_X)\text{ is finite}.}
$$

This is the surface case of [negative curves of a big real divisor lie in finitely many divisors](../../../cartier-divisor.md#negative-curves-of-a-big-real-divisor-lie-in-finitely-many-divisors). The proof does not assert that every negative curve on $X$ belongs to this finite set; it concerns curves negative against this particular big canonical class.

<h4 id="2/iv/b">b</h4>

↑ **Parent:** [Iv](#2/iv)

<h5 id="2/iv/b/solution">Solution</h5>

↑ **Parent:** [B](#2/iv/b)

Let $C\in\operatorname{Neg}(K_X)$. The [arithmetic adjunction formula on a smooth surface](../../../algebraic-geometry.md#arithmetic-adjunction-formula-on-a-smooth-surface) gives

$$
2p_a(C)-2=C^2+K_X\cdot C,\qquad p_a(C)\ge0.
$$

We first exclude $C^2\ge0$, following the PDF's hint and the finiteness proved in (a).

If $C^2=0$, adjunction and $K_X\cdot C<0$ force $p_a(C)=0$ and $K_X\cdot C=-2$. An integral projective curve of [arithmetic genus](../../../algebraic-geometry.md#arithmetic-genus) zero is a [smooth rational curve](../../../projective-space.md#smooth-rational-curve): normalization and the nonnegative singularity-length correction show both normalization genus and singularity correction vanish. Part (iii) makes $C$ [semiample](../../../cartier-divisor.md#semiample-divisor). Choose a basepoint-free $|mC|$. Over the infinite algebraically closed [field](../../../algebra.md#field), a general section avoids containing any of the finitely many curves of $\operatorname{Neg}(K_X)$ as a component. Its effective divisor $G$ then has $K_X\cdot G\ge0$, but $K_X\cdot G=mK_X\cdot C<0$, a contradiction.

If $C^2>0$, [Riemann–Roch theorem for algebraic surfaces](../../../algebraic-geometry.md#riemann-roch-theorem-for-algebraic-surfaces) and [Serre duality](../../../ringed-space.md#serre-duality) show $h^0(X,mC)$ is unbounded. Indeed $h^2(X,mC)=h^0(X,K_X-mC)=0$ for $m\gg0$, because the latter divisor has negative intersection with a fixed [ample](../../../ringed-space.md#ample-line-bundle) divisor. Hence

$$
h^0(X,mC)\ge\chi(X,\mathcal O_X)+\tfrac12(m^2C^2-mK_X\cdot C)\longrightarrow\infty.
$$

There is therefore some $m$ with $h^0(X,mC)>h^0(X,(m-1)C)$, giving a section whose divisor does not contain $C$. The canonical section of $mC$ does not vanish identically along any other curve. A general linear combination of these two sections consequently contains none of the finite set $\operatorname{Neg}(K_X)$, again contradicting its negative canonical intersection. Thus $C^2<0$.

Now put $a=-C^2\ge1$ and $b=-K_X\cdot C\ge1$. Adjunction gives

$$
-a-b=2p_a(C)-2\ge-2.
$$

It follows that $a=b=1$ and $p_a(C)=0$. Hence

$$
\boxed{C\cong\mathbb P^1,\qquad C^2=-1,\qquad K_X\cdot C=-1.}
$$

The general-section argument only avoids finitely many proper linear subspaces, so it works over any algebraically closed field, including positive characteristic.

<h4 id="2/iv/c">c</h4>

↑ **Parent:** [Iv](#2/iv)

<h5 id="2/iv/c/solution">Solution</h5>

↑ **Parent:** [C](#2/iv/c)

The [Castelnuovo contraction criterion](../../../algebraic-geometry.md#castelnuovo-contraction-criterion) says that a [smooth rational curve](../../../projective-space.md#smooth-rational-curve) $C$ on a [smooth projective surface](../../../algebraic-geometry.md#smooth-projective-surface) with $C^2=-1$ can be contracted by a [birational morphism](../../../algebraic-geometry.md#birational-morphism) to a smooth point of a [smooth projective surface](../../../algebraic-geometry.md#smooth-projective-surface). The contraction is an isomorphism away from $C$, and its inverse is the [blowup of a smooth algebraic surface](../../../algebraic-geometry.md#blowup-of-a-smooth-algebraic-surface) at that point. This is the algebraic contraction criterion, valid over the algebraically closed field here; it is not the rationality criterion bearing Castelnuovo's name.

By (b), every $C\in\operatorname{Neg}(K_X)$ satisfies the hypothesis. Therefore the required morphism exists:

$$
\boxed{f_1:X\to X_1,\quad f_1(C)=\{p\},\quad X_1\text{ smooth and projective},\quad X\setminus C\cong X_1\setminus\{p\}.}
$$

The PDF calls $f_1$ a birational map; the conclusion is stronger, since this map is everywhere defined and is a [birational morphism](../../../algebraic-geometry.md#birational-morphism).

## 3

↑ **Parent:** [Paper 134](paper-134.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

An [ample real divisor](../../../cartier-divisor.md#ample-real-divisor) is a finite positive real combination of [ample Cartier divisors](../../../cartier-divisor.md#ample-cartier-divisor):

$$
D=\sum_{j=1}^r a_jA_j,\qquad a_j>0.
$$

Equivalently its [numerical class](../../../cartier-divisor.md#real-numerical-divisor-classes) lies in the [ample cone](../../../cartier-divisor.md#ample-cone). This is a numerical condition even when the coefficients are irrational; it does not mean that some integer multiple of $D$ must be an integral divisor.

On an integral [projective variety](../../../projective-space.md#projective-variety), a [big real divisor](../../../cartier-divisor.md#big-real-divisor) is a finite positive real combination of [big Cartier divisors](../../../cartier-divisor.md#big-divisor). Equivalently, by the real form of [Kodaira's lemma](../../../cartier-divisor.md#kodaira-s-lemma),

$$
\boxed{D\sim_{\mathbb R}B+E,\quad B\text{ ample real},\quad E\text{ effective real Cartier}.}
$$

For an integral [Cartier divisor](../../../cartier-divisor.md), bigness means maximal section-growth order $h^0(X,mD)\ge c m^{\dim X}$ along sufficiently divisible positive $m$, or [Iitaka dimension](../../../cartier-divisor.md#iitaka-dimension) $\dim X$. The [real linear equivalence of divisors](../../../cartier-divisor.md#real-linear-equivalence-of-divisors) formulation permits finite positive combinations of effective [Cartier divisors](../../../cartier-divisor.md), whose supports are codimension one. The definitions and the ample-plus-effective formulation on integral varieties are discussed in [Fujino's notes on big real divisors](https://www.math.kyoto-u.ac.jp/~fujino/big-r-divisor5.pdf).

For the paper's assertions on a general [projective scheme](../../../ringed-space.md#projective-scheme), use [componentwise bigness on a projective scheme](../../../cartier-divisor.md#componentwise-bigness-on-a-projective-scheme): require bigness on every reduced irreducible component. All arguments below can then be carried out on those finitely many integral components; [ampleness](../../../cartier-divisor.md#ample-cartier-divisor) is also detected there. On a reducible scheme, merely asking for maximal total section growth on one component is insufficient. For example $X=\mathbb P^2\amalg\mathbb P^2$, with $D$ restricting to $\mathcal O(1)$ on the first component and $\mathcal O(-1)$ on the second, has quadratic total section growth, but negative intersection with every line in the second component. No finite collection of codimension-one [subvarieties](../../../algebraic-geometry.md#closed-subvariety) can contain all those lines. Thus that weaker meaning would make part (ii) false. In dimension zero the positivity statements are vacuous and every [line bundle](../../../ringed-space.md#line-bundle) is [ample](../../../ringed-space.md#ample-line-bundle); the compatible bigness convention also regards it as big.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

First work on an integral component. Write the [big real divisor](../../../cartier-divisor.md#big-real-divisor) as $D\sim_{\mathbb R}B+E$ with $B$ [ample real divisor](../../../cartier-divisor.md#ample-real-divisor) and $E$ effective real Cartier, using [Kodaira's lemma](../../../cartier-divisor.md#kodaira-s-lemma). Let $E_1,\ldots,E_k$ be the finitely many integral components of its support. For an integral [projective curve](../../../projective-space.md#projective-curve) $C$ not contained in this support, restriction of each effective Cartier summand to $C$ is effective, so

$$
D\cdot C=B\cdot C+E\cdot C>0.
$$

Therefore

$$
\boxed{D\cdot C<0\Longrightarrow C\subseteq E_i\text{ for some }i.}
$$

This proves [negative curves of a big real divisor lie in finitely many divisors](../../../cartier-divisor.md#negative-curves-of-a-big-real-divisor-lie-in-finitely-many-divisors).

Now let $A$ be the given [ample](../../../ringed-space.md#ample-line-bundle) divisor. Openness of the [ample cone](../../../cartier-divisor.md#ample-cone) gives a $\delta>0$ such that $B-\epsilon A$ is [ample](../../../ringed-space.md#ample-line-bundle) for $0<\epsilon\le\delta$. For each of the finitely many $E_i$, the assumption that $D|_{E_i}$ is [ample](../../../ringed-space.md#ample-line-bundle) similarly gives a $\delta_i>0$ such that $(D-\epsilon A)|_{E_i}$ is [ample](../../../ringed-space.md#ample-line-bundle) for $0<\epsilon\le\delta_i$. Choose a single positive $\epsilon$ smaller than all these bounds.

If $C$ is contained in some $E_i$, its intersection with $D-\epsilon A$ is positive by that restriction. Otherwise

$$
(D-\epsilon A)\cdot C=(B-\epsilon A)\cdot C+E\cdot C>0.
$$

In particular $D-\epsilon A$ is [nef](../../../cartier-divisor.md#nef-line-bundle):

$$
\boxed{D-\epsilon A\text{ is nef for all sufficiently small }\epsilon>0.}
$$

Only the finitely many exceptional support components are needed for the restriction test; no uniform bound over all [subvarieties](../../../algebraic-geometry.md#closed-subvariety) was assumed.

For a reducible [projective scheme](../../../ringed-space.md#projective-scheme), use [componentwise bigness on a projective scheme](../../../cartier-divisor.md#componentwise-bigness-on-a-projective-scheme) and repeat this argument on each reduced irreducible component. Collect their exceptional supports and take the minimum of all the finitely many positive bounds. Codimension one here is measured in the relevant irreducible component. Every integral curve lies in a component, so the same conclusion holds on $X$. Nilpotent structure does not affect these curve [intersection numbers](../../../algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve).

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/a">a</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/a/solution">Solution</h5>

↑ **Parent:** [A](#3/iii/a)

Take $V=C$ for each integral [projective curve](../../../projective-space.md#projective-curve) in $X$. The assumed positivity gives $D\cdot C>0$, hence certainly $D\cdot C\ge0$. By the definition of a [nef divisor](../../../cartier-divisor.md#nef-line-bundle),

$$
\boxed{D\in\operatorname{Nef}(X).}
$$

This is only the curve test. It does not already prove [ampleness](../../../cartier-divisor.md#ample-cartier-divisor): positivity against each individual curve can fail to be uniform on limiting classes in the [closed cone of curves](../../../cartier-divisor.md#closed-cone-of-curves). The hypotheses in higher dimensions, used in the next sections, are what rule out this failure.

<h4 id="3/iii/b">b</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/b/solution">Solution</h5>

↑ **Parent:** [B](#3/iii/b)

Choose an [ample Cartier divisor](../../../cartier-divisor.md#ample-cartier-divisor) $H$. Put initially $A=\delta H$, $A'=tH$ for small positive real $\delta,t$. Since $D$ is [nef](../../../cartier-divisor.md#nef-line-bundle), the [nef-plus-ample ampleness lemma](../../../cartier-divisor.md#nef-plus-ample-ampleness-lemma) makes $D+tH$ [ample](../../../ringed-space.md#ample-line-bundle). The polynomial

$$
P(\delta,t)=(D+tH)^n-n(D+tH)^{n-1}\cdot((\delta+t)H)
$$

has $P(0,0)=D^n\cdot[X]>0$. Thus the desired strict inequality holds when $\delta,t$ are sufficiently small and positive.

We must also arrange rationality of the two specified classes; $D$ itself need not be rational. Choose rational [ample](../../../ringed-space.md#ample-line-bundle) classes $B$ and $C$ sufficiently near $D+tH$ and $(\delta+t)H$, and define

$$
A'=B-D,\qquad A=C-A'=C-B+D.
$$

Then $A'$ is close to $tH$ and $A$ is close to $\delta H$, so both are [ample real divisors](../../../cartier-divisor.md#ample-real-divisor) by openness of the [ample cone](../../../cartier-divisor.md#ample-cone). Also $D+A'=B$ and $A+A'=C$ are rational and [ample](../../../ringed-space.md#ample-line-bundle). Continuity preserves the strict inequality, giving

$$
\boxed{B^n>nB^{n-1}\cdot C,\qquad D-A=B-C.}
$$

Here is the needed [algebraic Morse inequality for ample divisors](../../../cartier-divisor.md#algebraic-morse-inequality-for-ample-divisors), with its section-count proof. Choose rational [Cartier divisor](../../../cartier-divisor.md) representatives of $B,C$ and a common positive integer $q$ making $qB,qC$ [very ample](../../../ringed-space.md#very-ample-line-bundle) integral [Cartier divisors](../../../cartier-divisor.md). For the section-count argument rename these scaled representatives $B,C$; undoing this scaling restricts section indices to sufficiently divisible multiples and leaves bigness unchanged. Choose an effective [Cartier divisor](../../../cartier-divisor.md) $G\in|C|$ by taking a defining section that avoids the [associated points](../../../ringed-space.md#associated-point-of-a-coherent-sheaf) of $\mathcal O_X$. Repeated [divisor restriction exact sequences](../../../cartier-divisor.md#divisor-restriction-exact-sequence) give

$$
h^0(X,m(B-C))\ge h^0(X,mB)-\sum_{j=0}^{m-1}h^0(G,\mathcal O_G(mB-jC)).
$$

Because $C$ is [very ample](../../../ringed-space.md#very-ample-line-bundle), for each $j$ a section of $jC$ avoiding the finitely many [associated points](../../../ringed-space.md#associated-point-of-a-coherent-sheaf) of $\mathcal O_G$ gives an injection into $\mathcal O_G(mB)$. Thus every summand is at most $h^0(G,\mathcal O_G(mB))$. By [Serre vanishing](../../../ringed-space.md#serre-vanishing) and [asymptotic Riemann–Roch](../../../ringed-space.md#asymptotic-riemann-roch) for the [ample](../../../ringed-space.md#ample-line-bundle) $B$,

$$
h^0(X,m(B-C))\ge\frac{B^n-nB^{n-1}\cdot C}{n!}m^n+O(m^{n-1}).
$$

For $n=1$, the restriction term is the constant length of $G$, giving the same formula directly. The positive coefficient proves that $B-C$, hence $D-A$, is big. Scaling back preserves bigness, so

$$
\boxed{D-A\text{ is big}.}
$$

For a general [projective scheme](../../../ringed-space.md#projective-scheme), enforce the same strict inequality separately on each positive-dimensional reduced irreducible component $V_j$, using its own dimension $n_j$. At $(\delta,t)=(0,0)$ every such expression equals the positive number $D^{n_j}\cdot[V_j]$. Finitely many conditions are preserved by one sufficiently small choice and one sufficiently close rational approximation on $N^1(X)_{\mathbb R}$. The top-dimensional inequalities imply the printed inequality for $[X]$ with its positive generic multiplicities; the section proof on each component makes $D-A$ componentwise big. This avoids inferring bigness on every component from just a positive sum. The displayed inequality is used for $n\ge1$. For $n=0$, its literal $n-1$ intersection power is undefined; handle this vacuous positivity case separately. Every [line bundle](../../../ringed-space.md#line-bundle) is [ample](../../../ringed-space.md#ample-line-bundle), all [numerical classes](../../../cartier-divisor.md#real-numerical-divisor-classes) are zero, and the componentwise bigness convention makes the conclusions automatic.

<h4 id="3/iii/c">c</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/c/solution">Solution</h5>

↑ **Parent:** [C](#3/iii/c)

Part (b) supplies an [ample](../../../ringed-space.md#ample-line-bundle) $A$ with $D-A$ big. Therefore $D=(D-A)+A$ is big as well, since adding an [ample](../../../ringed-space.md#ample-line-bundle) class to a big class preserves the ample-plus-effective decomposition. The permitted induction hypothesis makes $D$ [ample](../../../ringed-space.md#ample-line-bundle) on every proper positive-dimensional closed subscheme of lower dimension, in particular on every codimension-one integral [subvariety](../../../algebraic-geometry.md#closed-subvariety). Zero-dimensional restrictions are [ample](../../../ringed-space.md#ample-line-bundle) automatically.

Apply part (ii) to this big $D$ and the [ample](../../../ringed-space.md#ample-line-bundle) $A$ chosen in (b). The result is

$$
\boxed{D-\epsilon A\text{ is nef for }0<\epsilon\ll1.}
$$

For a reducible scheme the same argument is componentwise. If a positive-dimensional irreducible component itself is a strict closed subscheme of $X$, the permitted induction assumption already makes $D$ [ample](../../../ringed-space.md#ample-line-bundle) on that component; otherwise its codimension-one [subvarieties](../../../algebraic-geometry.md#closed-subvariety) are lower-dimensional and the same proof applies. Only one finite minimum of bounds is required.

<h4 id="3/iii/d">d</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/d/solution">Solution</h5>

↑ **Parent:** [D](#3/iii/d)

Choose $0<\epsilon\ll1$ as in (c). Then

$$
D=(D-\epsilon A)+\epsilon A
$$

is the sum of a [nef divisor](../../../cartier-divisor.md#nef-line-bundle) and an [ample real divisor](../../../cartier-divisor.md#ample-real-divisor). The [nef-plus-ample ampleness lemma](../../../cartier-divisor.md#nef-plus-ample-ampleness-lemma) gives

$$
\boxed{D\text{ is ample}.}
$$

For clarity, this last lemma follows from [Kleiman's criterion](../../../cartier-divisor.md#kleiman-s-criterion) and the [convex cone](../../../mathematical-optimization.md#convex-cone) property: if $x$ is an interior point of the [nef cone](../../../cartier-divisor.md#nef-cone) and $y$ lies in that cone, translating a small neighbourhood of $x$ by $y$ stays in the cone. Thus $x+y$ remains in its interior, which is the [ample cone](../../../cartier-divisor.md#ample-cone) on a [projective scheme](../../../ringed-space.md#projective-scheme).

The complete argument proves the [real Nakai–Moishezon criterion](../../../cartier-divisor.md#real-nakai-moishezon-criterion) rather than assuming it: curve positivity gives nefness, rational approximation and a proved section-count inequality give bigness, induction and the finite-support argument give a uniform [ample](../../../ringed-space.md#ample-line-bundle) subtraction, and the nef-plus-ample lemma concludes [ampleness](../../../cartier-divisor.md#ample-cartier-divisor). The zero-dimensional case is automatic, and [ampleness on reduced components](../../../ringed-space.md#ampleness-on-reduced-components) handles reducibility and nilpotents.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
