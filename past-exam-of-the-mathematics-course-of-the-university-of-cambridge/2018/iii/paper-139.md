# Paper 139

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_139.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_139.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
- [2](#2)
  - [i](#2/i)
    - [a](#2/i/a)
      - [Solution](#2/i/a/solution)
    - [b](#2/i/b)
      - [Solution](#2/i/b/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
  - [vi](#2/vi)
    - [a](#2/vi/a)
      - [Solution](#2/vi/a/solution)
    - [b](#2/vi/b)
      - [Solution](#2/vi/b/solution)
  - [vii](#2/vii)
    - [Solution](#2/vii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [a](#3/v/a)
      - [Solution](#3/v/a/solution)
    - [b](#3/v/b)
      - [Solution](#3/v/b/solution)
    - [c](#3/v/c)
      - [Solution](#3/v/c/solution)
  - [vi](#3/vi)
    - [Solution](#3/vi/solution)

## 1

↑ **Parent:** [Paper 139](paper-139.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For a [projective scheme](../../../ringed-space.md#projective-scheme) $X$ of [dimension of a scheme](../../../ringed-space.md#dimension-of-a-scheme) $n$ and a [Cartier divisor](../../../cartier-divisor.md) $D$, [asymptotic Riemann–Roch](../../../ringed-space.md#asymptotic-riemann-roch) gives

$$
\boxed{\chi(X,\mathcal O_X(mD))=\frac{D^n}{n!}m^n+O(m^{n-1}).}
$$

Here [Euler characteristic of a coherent sheaf](../../../ringed-space.md#euler-characteristic-of-a-coherent-sheaf) means $\chi=\sum_{i=0}^n(-1)^ih^i$, and $D^n$ is the degree of the top [intersection product](../../../algebraic-geometry.md#intersection-product-of-cartier-divisors) with the fundamental cycle of $X$, including its component multiplicities. No [ampleness](../../../cartier-divisor.md#ample-cartier-divisor) assumption on $D$ is needed.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [Nakai–Moishezon criterion](../../../cartier-divisor.md#nakai-moishezon-criterion) says that a [Cartier divisor](../../../cartier-divisor.md) $D$ on a [projective scheme](../../../ringed-space.md#projective-scheme) is [ample](../../../ringed-space.md#ample-line-bundle) exactly when

$$
D^{\dim Y}\cdot Y>0
$$

for every positive-dimensional integral closed [subvariety](../../../algebraic-geometry.md#closed-subvariety) $Y$. [Kleiman's criterion](../../../cartier-divisor.md#kleiman-s-criterion) says that the [ample cone](../../../cartier-divisor.md#ample-cone) is the interior of the [nef cone](../../../cartier-divisor.md#nef-cone); equivalently, the [numerical class](../../../cartier-divisor.md#real-numerical-divisor-classes) of $D$ is ample exactly when it is strictly positive on every nonzero element of the [closed cone of curves](../../../cartier-divisor.md#closed-cone-of-curves) $\overline{\operatorname{NE}}(X)$. Positivity merely on individual curves is insufficient: the closure of the cone is essential. A [nef divisor](../../../cartier-divisor.md#nef-line-bundle) has nonnegative [intersection number](../../../algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve) with every integral curve, and its restriction to every closed subscheme is nef.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Choose [very ample divisors](../../../cartier-divisor.md#very-ample-divisor) $H_2$ and $H_1\sim D+H_2$, with defining sections avoiding the [associated points](../../../ringed-space.md#associated-point-of-a-coherent-sheaf) of $X$. Such a choice is possible after taking a sufficiently high ample twist. Put $R_m=mD-H_1=(m-1)D-H_2$. The two indicated [short exact sequences of sheaves](../../../algebraic-geometry.md#short-exact-sequence-of-sheaves) and their [long exact sequences in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology) imply

$$
h^j(X,mD)\leq h^j(X,(m-1)D)+h^j(H_1,mD)+h^{j-1}(H_2,(m-1)D).
$$

We abbreviate $h^i(Z,\mathcal O_Z(L))$ by $h^i(Z,L)$. Each $H_a$ has dimension $n-1$ and the restricted divisor is [nef](../../../cartier-divisor.md#nef-line-bundle). For positive degrees below $n-1$, the assumed induction estimate bounds the error terms by $O(m^{n-2})$. The displayed hypothesis omits top-degree cohomology; use [top cohomology boundedness for nef twists](../../../ringed-space.md#top-cohomology-boundedness-for-nef-twists) for that degree, and [Grothendieck vanishing](../../../ringed-space.md#grothendieck-vanishing) above it. These give the same error bound. The auxiliary top-degree result follows from [Fujita vanishing](../../../ringed-space.md#fujita-vanishing) by cutting a [coherent sheaf](../../../ringed-space.md#coherent-sheaf) with an ample divisor, as proved in [cohomology growth for nef twists](../../../ringed-space.md#cohomology-growth-for-nef-twists).

For $n\geq2$, summing the inequality over successive $m$ gives $h^j(X,mD)=O(m^{n-1})$ for every $j>1$. For $n\leq1$, all such groups vanish by [Grothendieck vanishing](../../../ringed-space.md#grothendieck-vanishing).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

By [asymptotic Riemann–Roch](../../../ringed-space.md#asymptotic-riemann-roch) and the preceding bounds for higher [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology),

$$
\boxed{h^0(X,mD)-h^1(X,mD)=\frac{D^n}{n!}m^n+O(m^{n-1}).}
$$

A [nef divisor](../../../cartier-divisor.md#nef-line-bundle) satisfies $D^n\geq0$: for a fixed [ample divisor](../../../cartier-divisor.md#ample-cartier-divisor) $A$, the divisors $D+\varepsilon A$ are ample for positive rational $\varepsilon$, and continuity of the [intersection product](../../../algebraic-geometry.md#intersection-product-of-cartier-divisors) gives the inequality as $\varepsilon\to0$. If $h^0(X,mD)=0$ eventually, the left side is nonpositive. Dividing by $m^n$ forces $D^n=0$, since $h^1\geq0$ and $D^n\geq0$. The same identity then gives $h^1(X,mD)=O(m^{n-1})$.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

First suppose $X$ is integral. Induct on its [dimension of a scheme](../../../ringed-space.md#dimension-of-a-scheme). The previous two parts handle all $j>1$ and also handle $j=1$ when $h^0(X,mD)$ eventually vanishes. Otherwise choose $r>0$ with a nonzero [global section](../../../ringed-space.md#global-section) of $rD$. On an integral variety it defines an [effective Cartier divisor](../../../cartier-divisor.md#effective-cartier-divisor) $E$, possibly empty, and multiplication by the section gives

$$
0\to\mathcal O_X((m-r)D)\to\mathcal O_X(mD)\to\mathcal O_E(mD)\to0.
$$

Thus $h^1(X,mD)\leq h^1(X,(m-r)D)+h^1(E,mD)$. For $n\geq2$, the induction hypothesis bounds the last term by $O(m^{n-2})$; summing on each residue class modulo $r$ gives $O(m^{n-1})$. For $n=1$, $E$ is zero-dimensional and its positive-degree [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) vanishes, so the same recurrence is bounded.

For a general [projective scheme](../../../ringed-space.md#projective-scheme), a nonzero section can be a [zero divisor](../../../mathematics.md#zero-divisor), so that argument requires an additional step. The general [cohomology growth for nef twists](../../../ringed-space.md#cohomology-growth-for-nef-twists) supplies it: for every [coherent sheaf](../../../ringed-space.md#coherent-sheaf) $\mathcal F$ with support dimension $d$,

$$
h^i(X,\mathcal F\otimes\mathcal O_X(mD))=O(m^{d-i})\quad(1\leq i\leq d).
$$

Its proof uses [Fujita vanishing](../../../ringed-space.md#fujita-vanishing), an ample section avoiding the [associated points](../../../ringed-space.md#associated-point-of-a-coherent-sheaf) of $\mathcal F$, and induction on support dimension. Taking $\mathcal F=\mathcal O_X$ gives the required $O(m^{n-1})$ estimate for every $j\geq1$, including nonreduced and reducible schemes; degrees above $n$ vanish.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

The divisor is understood to be on $X$; the printed “on $D$” is a typo. Combining [asymptotic Riemann–Roch](../../../ringed-space.md#asymptotic-riemann-roch) with [cohomology growth for nef twists](../../../ringed-space.md#cohomology-growth-for-nef-twists) gives

$$
h^0(X,\mathcal O_X(mD))=\frac{D^n}{n!}m^n+O(m^{n-1}),\qquad
\boxed{\lim_{m\to\infty}\frac{h^0(X,\mathcal O_X(mD))}{m^n}=\frac{D^n}{n!}.}
$$

Since a [nef divisor](../../../cartier-divisor.md#nef-line-bundle) has nonnegative top [self-intersection number](../../../algebraic-geometry.md#self-intersection-number), this [limit](../../../calculus.md#limit-of-a-function) is positive exactly when $D^n>0$. This is the [volume of a nef divisor](../../../cartier-divisor.md#volume-of-a-nef-divisor) criterion.

## 2

↑ **Parent:** [Paper 139](paper-139.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/a">a</h4>

↑ **Parent:** [I](#2/i)

<h5 id="2/i/a/solution">Solution</h5>

↑ **Parent:** [A](#2/i/a)

Write $F=\sum_C\min_{G\in|H|}\operatorname{mult}_C(G)\,C$. This is the [fixed part of a linear system](../../../cartier-divisor.md#fixed-part-of-a-linear-system). The [movable part of a linear system](../../../cartier-divisor.md#movable-part-of-a-linear-system) is $|M|$, with $M=H-F$; multiplication by the defining section of $F$ identifies its sections with those of $H$. In particular $|H|=F+|M|$, and no curve occurs in every member of $|M|$. The occurrence of $|F|$ in the definition request is understood as $|H|$.

For any integral curve $C$, choose a member $G\in|M|$ not containing $C$. Their [intersection number](../../../algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve) is a sum of nonnegative local [intersection multiplicities](../../../algebraic-geometry.md#intersection-multiplicity), so $M\cdot C=G\cdot C\geq0$. Therefore **the movable divisor $M$ is nef**. If $M=0$, the same assertion is immediate.

<h4 id="2/i/b">b</h4>

↑ **Parent:** [I](#2/i)

<h5 id="2/i/b/solution">Solution</h5>

↑ **Parent:** [B](#2/i/b)

The relevant invariant of a divisor is its [Iitaka dimension](../../../cartier-divisor.md#iitaka-dimension), also called its Kodaira dimension. If two linearly independent [global sections](../../../ringed-space.md#global-section) $s,t$ occur in $H^0(X,nH)$, their ratio is a nonconstant [rational function](../../../isolated-singularity.md#rational-function). The sections $s^q,s^{q-1}t,\ldots,t^q$ are linearly independent, because a nonconstant rational function over an algebraically closed field is transcendental over that field. Thus some [complete linear system of a divisor](../../../cartier-divisor.md#complete-linear-system-of-a-divisor) has positive-dimensional image, contradicting $\kappa(H)=0$.

Consequently $h^0(X,nH)=1$ for every $n>0$; the nonemptiness of $|H|$ supplies a nonzero section in every multiple. Its unique divisor is entirely fixed. Hence **every movable part $M_n$ is zero**.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Because $|D|$ has no [fixed components](../../../cartier-divisor.md#fixed-component), choose two members $G_1,G_2$ with no common component. This uses the infinitude of the algebraically closed field and avoidance of finitely many proper linear subspaces of the section space. On a [smooth algebraic surface](../../../algebraic-geometry.md#smooth-algebraic-surface), their [intersection number](../../../algebraic-geometry.md#intersection-number-of-a-cartier-divisor-with-a-curve) is the sum of local [intersection multiplicities](../../../algebraic-geometry.md#intersection-multiplicity). Since $G_1\cdot G_2=D^2=0$, they are disjoint. A basepoint of $|D|$ would belong to both, so **$|D|$ is basepoint-free**.

The resulting [morphism](../../../algebra.md#morphism) has nonconstant image since $\dim|D|\geq1$. Its image cannot be a surface: a generically finite morphism defined by $D$ would make $D^2$ the positive product of its degree and the degree of its image. Thus the image is a curve. Apply [Stein factorization](../../../ringed-space.md#stein-factorization) to obtain $g:X\to C$ with connected fibers and $g_*\mathcal O_X=\mathcal O_C$, where $C$ is a smooth projective curve. There is a positive-degree [line bundle](../../../ringed-space.md#line-bundle) $L$ on $C$ with $\mathcal O_X(D)=g^*L$. The [projection formula for sheaves](../../../ringed-space.md#projection-formula) and [Riemann-Roch theorem](../../../algebraic-geometry.md#riemann-roch-theorem) give $h^0(X,mD)=h^0(C,L^m)=m\deg L+O(1)$. Therefore

$$
\boxed{\kappa(D)=1.}
$$

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Each $M_n$ is a [nef divisor](../../../cartier-divisor.md#nef-line-bundle). If $M_n^2>0$, the [volume of a nef divisor](../../../cartier-divisor.md#volume-of-a-nef-divisor) formula gives quadratic growth of $h^0(X,qM_n)$. Multiplication by the section of $qF_n$ injects this space into $H^0(X,qnH)$, so the [birational linear system criterion for bigness](../../../cartier-divisor.md#birational-linear-system-criterion-for-bigness) makes the [Iitaka dimension](../../../cartier-divisor.md#iitaka-dimension) of $H$ two.

Conversely, if $\kappa(H)=2$, some $|nH|$, and hence its [movable part](../../../cartier-divisor.md#movable-part-of-a-linear-system) $|M_n|$, has a two-dimensional image. If $M_n^2=0$, the previous part would make $|M_n|$ basepoint-free with image a curve; this is impossible. Since $M_n$ is nef, $M_n^2\geq0$, hence $M_n^2>0$.

If all $M_n^2=0$ and one $|M_{n'}|$ has positive dimension, the preceding part supplies a curve image. The just-proved equivalence excludes dimension two, so $\kappa(H)=1$. Conversely $\kappa(H)=1$ excludes every positive $M_n^2$ and requires a positive-dimensional linear system. Thus

$$
\boxed{\kappa(H)=2\iff (\exists n)\ M_n^2>0,\qquad
\kappa(H)=1\iff (\forall n)\ M_n^2=0\ \text{and}\ (\exists n')\ \dim|M_{n'}|\geq1.}
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

A connected integral [projective variety](../../../projective-space.md#projective-variety) has only constant regular functions, so $h^0(X,\mathcal O_X)=1$. By [Serre duality](../../../ringed-space.md#serre-duality) and $K_X\sim0$, $h^2(X,\mathcal O_X)=h^0(X,\mathcal O_X(K_X))=1$. The assumed first [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) vanishes. Therefore the [Euler characteristic of a coherent sheaf](../../../ringed-space.md#euler-characteristic-of-a-coherent-sheaf) is

$$
\boxed{\chi(X,\mathcal O_X)=1-0+1=2.}
$$

These hypotheses characterize the [K3 surface](../../../complex-geometry.md#k3-surface) setting used below.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

Choose an [ample divisor](../../../cartier-divisor.md#ample-cartier-divisor) $A$. The [Hodge index theorem for algebraic surfaces](../../../algebraic-geometry.md#hodge-index-theorem-for-algebraic-surfaces) implies $D\cdot A>0$: if it were zero, $D^2=0$ would force the [numerical class](../../../cartier-divisor.md#real-numerical-divisor-classes) of $D$ to be zero. Consequently $-D$ cannot be effective, because every nonzero [effective divisor](../../../cartier-divisor.md#effective-cartier-divisor) has positive intersection with $A$, while $-D\cdot A<0$.

The [Riemann–Roch theorem for algebraic surfaces](../../../algebraic-geometry.md#riemann-roch-theorem-for-algebraic-surfaces) and the preceding computation give $\chi(X,\mathcal O_X(D))=2+D^2/2=2$. By [Serre duality](../../../ringed-space.md#serre-duality), $h^2(X,D)=h^0(X,-D)=0$. Thus

$$
\boxed{h^0(X,D)=2+h^1(X,D)\geq2.}
$$

<h3 id="2/vi">vi</h3>

↑ **Parent:** [2](#2)

<h4 id="2/vi/a">a</h4>

↑ **Parent:** [Vi](#2/vi)

<h5 id="2/vi/a/solution">Solution</h5>

↑ **Parent:** [A](#2/vi/a)

First derive the intersection constraints. Since $D$ is [nef](../../../cartier-divisor.md#nef-line-bundle) and $F,M$ are effective, $D\cdot F,D\cdot M\geq0$; their sum is $D^2=0$, so both vanish. Since the [movable divisor](../../../cartier-divisor.md#movable-part-of-a-linear-system) $M$ is nef, $M^2,M\cdot F\geq0$, and $M\cdot D=0$ forces both to vanish. In particular

$$
D\cdot F=D\cdot M=M^2=M\cdot F=F^2=0.
$$

For every component $E$ of $F$, nefness and $D\cdot F=0$ imply $D\cdot E=0$. The [isotropic orthogonality consequence of the Hodge index theorem](../../../algebraic-geometry.md#isotropic-orthogonality-consequence-of-the-hodge-index-theorem) gives $E^2\leq0$. If $E^2=0$, [Riemann–Roch theorem for algebraic surfaces](../../../algebraic-geometry.md#riemann-roch-theorem-for-algebraic-surfaces) and [Serre duality](../../../ringed-space.md#serre-duality) give $h^0(X,E)\geq2$, since $-E$ cannot be effective. Choose $E'\in|E|$ different from $E$. It cannot contain $E$: otherwise $E'-E$ would be a nonzero effective numerically trivial divisor, contradicting its positive intersection with an ample divisor. Choose a member of $|M|$ avoiding $E$. Replacing one copy of $E$ in $F$ by $E'$ now produces a member of $|D|$ with smaller multiplicity along $E$, contradicting the definition of the [fixed part](../../../cartier-divisor.md#fixed-part-of-a-linear-system). Therefore

$$
\boxed{E^2<0\quad\text{for every component of }F.}
$$

<h4 id="2/vi/b">b</h4>

↑ **Parent:** [Vi](#2/vi)

<h5 id="2/vi/b/solution">Solution</h5>

↑ **Parent:** [B](#2/vi/b)

The strict statement as printed needs the qualification **if $F\ne0$**. Part (a) already shows $F^2=0$ in the present situation, and the next part proves $F=0$; an unconditional $F^2<0$ would contradict that conclusion.

To prove the needed conditional statement, suppose $F\ne0$. A [fixed part](../../../cartier-divisor.md#fixed-part-of-a-linear-system) has $h^0(X,F)=1$. Indeed, a different $F'\in|F|$ has smaller multiplicity along some component of $F$; otherwise $F'-F$ would be a nonzero effective linearly trivial divisor. Adding a member of the [movable part](../../../cartier-divisor.md#movable-part-of-a-linear-system) avoiding that component contradicts fixedness.

The [Hodge index theorem for algebraic surfaces](../../../algebraic-geometry.md#hodge-index-theorem-for-algebraic-surfaces), together with $D\cdot F=0$ and $D^2=0$, gives $F^2\leq0$. If equality held, [Riemann–Roch theorem for algebraic surfaces](../../../algebraic-geometry.md#riemann-roch-theorem-for-algebraic-surfaces) would give $\chi(X,F)=2$, and [Serre duality](../../../ringed-space.md#serre-duality) would give $h^2(X,F)=h^0(X,-F)=0$. Hence $h^0(X,F)=2+h^1(X,F)\geq2$, a contradiction. Therefore

$$
\boxed{F\ne0\ \Longrightarrow\ F^2<0.}
$$

This is the [fixed-part elimination on a K3 surface](../../../complex-geometry.md#fixed-part-elimination-on-a-k3-surface) argument.

<h3 id="2/vii">vii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#2/vii)

The intersection calculation in part (vi)(a) gives $F^2=0$. Part (vi)(b), with its necessary $F\ne0$ qualification, excludes every nonzero fixed part. Thus $F=0$ and $|D|$ is movable. Part (v) gives $\dim|D|\geq1$, and $D^2=0$ by hypothesis. Applying part (ii) proves

$$
\boxed{|D|\text{ is basepoint-free},\qquad\kappa(D)=1.}
$$

Thus a nontrivial [nef divisor](../../../cartier-divisor.md#nef-line-bundle) of square zero on a [K3 surface](../../../complex-geometry.md#k3-surface) defines a fibration over a curve; the key step is [fixed-part elimination on a K3 surface](../../../complex-geometry.md#fixed-part-elimination-on-a-k3-surface).

## 3

↑ **Parent:** [Paper 139](paper-139.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Choose a [very ample divisor](../../../cartier-divisor.md#very-ample-divisor) $A$ such that $A-D$ has a nonzero [global section](../../../ringed-space.md#global-section); this is possible by taking a sufficiently high ample twist. Since $X$ is integral, multiplication by its $m$th power injects $H^0(X,mD)$ into $H^0(X,mA)$. By [Serre vanishing](../../../ringed-space.md#serre-vanishing) and the [Hilbert polynomial](../../../algebraic-geometry.md#hilbert-polynomial), $h^0(X,mA)=O(m^n)$. Consequently

$$
\boxed{h^0(X,mD)\leq C m^n\quad(m\gg0).}
$$

This is the [polynomial bound for sections of a fixed divisor](../../../algebraic-geometry.md#polynomial-bound-for-sections-of-a-fixed-divisor). The same proof works for a [coherent sheaf](../../../ringed-space.md#coherent-sheaf) of support dimension $d$, by choosing the multiplying section to avoid its [associated points](../../../ringed-space.md#associated-point-of-a-coherent-sheaf); the bound is then $O(m^d)$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For an [effective Cartier divisor](../../../cartier-divisor.md#effective-cartier-divisor) $F$, the [divisor restriction exact sequence](../../../cartier-divisor.md#divisor-restriction-exact-sequence) gives

$$
0\to\mathcal O_X(kD-F)\to\mathcal O_X(kD)\to\mathcal O_F(kD)\to0.
$$

The scheme $F$ has dimension at most $n-1$, so the permitted scheme version of part (i) bounds $h^0(F,\mathcal O_F(kD))$ by $Ck^{n-1}$. For the infinitely many $k$ in the hypothesis,

$$
h^0(X,kD-F)\geq C'k^n-Ck^{n-1}>0
$$

once $k$ is sufficiently large. Thus **infinitely many such $k$ have a nonzero section of $kD-F$**. This dimension-drop argument is the [section subtraction lemma for big divisors](../../../cartier-divisor.md#section-subtraction-lemma-for-big-divisors).

If “effective divisor” is interpreted as an effective [Weil divisor](../../../algebraic-geometry.md#weil-divisor) on a normal variety, use its coherent divisor ideal instead. The quotient by that ideal is supported in dimension at most $n-1$, so the [polynomial bound for sections of a fixed divisor](../../../algebraic-geometry.md#polynomial-bound-for-sections-of-a-fixed-divisor) gives the same conclusion. For $F=0$ the assertion is immediate.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Fix any [ample divisor](../../../cartier-divisor.md#ample-cartier-divisor) $A$. Choose $q\gg0$ so that both $qA$ and $(q-1)A$ have nonzero [global sections](../../../ringed-space.md#global-section), and choose $F\in|qA|$. Condition (1) and the [section subtraction lemma for big divisors](../../../cartier-divisor.md#section-subtraction-lemma-for-big-divisors) yield an integer $j>0$ with $jD-qA\sim E_0\geq0$. Adding an effective member of $|(q-1)A|$ gives $jD\sim A+E$. Thus (1) implies the stronger condition (2').

If $jD\sim A+E$ with $A$ ample and $E$ effective, multiplication by the section of $qE$ injects $H^0(X,qA)$ into $H^0(X,qjD)$. The positive leading coefficient of the ample [Hilbert polynomial](../../../algebraic-geometry.md#hilbert-polynomial) supplies condition (1) along the infinite sequence $m=qj$. Condition (2) implies (3). Conversely, if $jD\equiv A+E$, put $P=jD-E$. The [Cartier divisor](../../../cartier-divisor.md) $P$ is numerically equivalent to $A$, hence ample by [Kleiman's criterion](../../../cartier-divisor.md#kleiman-s-criterion); the actual equality $jD=P+E$ gives (2).

We have proved (1)$\Rightarrow$(2')$\Rightarrow$(2)$\Rightarrow$(1), and (3)$\Rightarrow$(2)$\Rightarrow$(3). Also (2') implies (3'), while (3') implies (3). Hence **all five conditions are equivalent**. They characterize a [big divisor](../../../cartier-divisor.md#big-divisor); the ample-plus-effective formulation is [Kodaira's lemma](../../../cartier-divisor.md#kodaira-s-lemma). The inconsistent use of $n$ and $j$ in the printed multiplier is resolved by using $j$ throughout.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Choose a [very ample divisor](../../../cartier-divisor.md#very-ample-divisor) $A$. By the stronger form of [Kodaira's lemma](../../../cartier-divisor.md#kodaira-s-lemma), $jD\sim A+E$ for some effective divisor $E$. The subsystem $s_EH^0(X,A)\subseteq H^0(X,jD)$ defines the embedding given by $A$ on $X\setminus\operatorname{Supp}E$. Ratios of its sections generate the [function field](../../../algebraic-geometry.md#function-field-of-an-algebraic-variety) $k(X)$. The map from the complete [complete linear system of a divisor](../../../cartier-divisor.md#complete-linear-system-of-a-divisor) contains these ratios, so it induces the same function field and is **birational onto its image**.

**The converse is true; smoothness is unnecessary.** If $|jD|$ gives a birational map, choose $n$ algebraically independent ratios $s_1/s_0,\ldots,s_n/s_0$ among a generating set of its section ratios. For every $q$, the sections

$$
s_0^{q-|\alpha|}\prod_{i=1}^ns_i^{\alpha_i},\qquad \alpha\in\mathbb N^n,\quad |\alpha|\leq q,
$$

are linearly independent by [algebraic independence](../../../algebra.md#algebraic-independence). Therefore $h^0(X,qjD)\geq\binom{q+n}{n}$, giving condition (1) of part (iii). This is the [birational linear system criterion for bigness](../../../cartier-divisor.md#birational-linear-system-criterion-for-bigness).

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/a">a</h4>

↑ **Parent:** [V](#3/v)

<h5 id="3/v/a/solution">Solution</h5>

↑ **Parent:** [A](#3/v/a)

Condition (a) is the definition of a [big real divisor](../../../cartier-divisor.md#big-real-divisor). Fix an ample Cartier divisor $A$. For each big Cartier divisor $D_i$, part (iii) gives $j_iD_i\sim A+E_i$ with $E_i$ effective. Consequently

$$
D\sim_{\mathbb R}\left(\sum_i\frac{d_i}{j_i}\right)A+\sum_i\frac{d_i}{j_i}E_i.
$$

The first coefficient is positive, proving (b).

For the converse, suppose $D\sim_{\mathbb R}tA+E$, with $t>0$ and $E$ effective. Apply [rational approximation of an ample-plus-effective real divisor](../../../cartier-divisor.md#rational-approximation-of-an-ample-plus-effective-real-divisor): in a finite-dimensional space generated by Cartier divisors and the finitely many principal divisors occurring in this relation, express $D$ as a positive convex combination of rational divisors $B_\nu$, each satisfying $B_\nu\sim_{\mathbb Q}t_\nu A+E_\nu$ with $t_\nu>0$ and $E_\nu$ effective. After clearing denominators, part (iii) shows that each $B_\nu$ is a positive rational multiple of a big Cartier divisor. This gives the actual equality required by (a), rather than merely a numerical or linear equivalence.

The approximation lemma keeps the finitely many effectivity inequalities and linear-equivalence equations simultaneously; see its proof for the rational-face argument and the reduction of nonnormal varieties by finite normalization. Therefore **(a) and (b) are equivalent**.

<h4 id="3/v/b">b</h4>

↑ **Parent:** [V](#3/v)

<h5 id="3/v/b/solution">Solution</h5>

↑ **Parent:** [B](#3/v/b)

Condition (b) immediately implies (c): a positive real multiple $tA$ of an [ample divisor](../../../cartier-divisor.md#ample-cartier-divisor) is an [ample real divisor](../../../cartier-divisor.md#ample-real-divisor), and [real linear equivalence of divisors](../../../cartier-divisor.md#real-linear-equivalence-of-divisors) implies [numerical equivalence of divisors](../../../cartier-divisor.md#numerical-equivalence-of-divisors).

More explicitly, the real numerical class of $D$ is the sum of a class in the [ample cone](../../../cartier-divisor.md#ample-cone) and an effective real divisor class. This separates strict positivity from the possibly degenerate effective part; it does not claim that the effective part itself is ample.

<h4 id="3/v/c">c</h4>

↑ **Parent:** [V](#3/v)

<h5 id="3/v/c/solution">Solution</h5>

↑ **Parent:** [C](#3/v/c)

Suppose $D\equiv A'+E'$ as in (c), and set $P=D-E'$. Its numerical class is ample, so $P$ is an [ample real divisor](../../../cartier-divisor.md#ample-real-divisor). Fix an ample Cartier divisor $A$. The [ample cone](../../../cartier-divisor.md#ample-cone) is open by [Kleiman's criterion](../../../cartier-divisor.md#kleiman-s-criterion), so choose $\varepsilon>0$ with $P-\varepsilon A$ still ample. Express this ample real divisor as a positive real combination $\sum b_iB_i$ of ample Cartier divisors. Some positive multiple of each $B_i$ has an effective representative; dividing by that multiple gives $B_i\sim_{\mathbb Q}G_i$ with $G_i$ effective. Hence

$$
D\sim_{\mathbb R}\varepsilon A+\left(E'+\sum_i b_iG_i\right),
$$

which is (b). The equivalence of numerical ampleness with a positive combination of ample Cartier representatives follows by rational approximation inside the open ample cone; the [rational approximation of an ample-plus-effective real divisor](../../../cartier-divisor.md#rational-approximation-of-an-ample-plus-effective-real-divisor) proof also accounts for principal-divisor directions.

Finally, if $D'\equiv D$, the same expression $D'\equiv A'+E'$ satisfies (c). By the equivalences just proved, $D'$ satisfies all three conditions exactly when $D$ does. Thus **bigness is invariant under numerical equivalence**, for real as well as Cartier divisors.

<h3 id="3/vi">vi</h3>

↑ **Parent:** [3](#3)

<h4 id="3/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#3/vi)

The space of [real numerical divisor classes](../../../cartier-divisor.md#real-numerical-divisor-classes) is $N^1(X)_{\mathbb R}$. Write any big class as $[D]=[A]+[E]$, with $A$ an [ample real divisor](../../../cartier-divisor.md#ample-real-divisor) and $E$ effective. For a sufficiently small perturbation $\delta\in N^1(X)_{\mathbb R}$, the class $[A]+\delta$ remains in the open [ample cone](../../../cartier-divisor.md#ample-cone), so $[D]+\delta$ remains big by part (v). Thus $\operatorname{Big}(X)$ is open. Positive scaling and addition preserve the ample-plus-effective expression, so it is a [convex cone](../../../mathematical-optimization.md#convex-cone).

For $n\geq1$, fix a very ample divisor $H$. The linear functional $\ell([D])=D\cdot H^{n-1}$ is strictly positive on every big class: the ample part contributes positively and the effective part nonnegatively. No nonzero linear subspace can be contained in this cone, since it would contain both $v$ and $-v$. In particular the zero class is not big in positive dimension. When $n=0$, $N^1(X)_{\mathbb R}=0$, so there is no positive-dimensional subspace to consider. Therefore

$$
\boxed{\operatorname{Big}(X)\text{ is an open convex cone and contains no positive-dimensional vector subspace}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
