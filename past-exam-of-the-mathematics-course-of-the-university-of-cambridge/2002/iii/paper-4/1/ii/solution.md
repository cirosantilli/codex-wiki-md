<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $e=1$ and write $G_{\geq e}$ for the nonnegative cone, including the identity. Every element of this cone is its own [absolute value in a lattice-ordered group](../../../../../../absolute-value-in-a-lattice-ordered-group.md), so the desired condition is equivalent to

$$
ab\leq b^2a^2\qquad(a,b\in G_{\geq e}).\qquad\text{(1)}
$$

We prove this equivalence with [normal-valued lattice-ordered group](../../../../../../normal-valued-lattice-ordered-group.md) without assuming any characterization of normal values. Membership of $g$ in a [convex lattice subgroup](../../../../../../convex-lattice-subgroup.md) is equivalent to membership of $|g|$, so it suffices to discuss values of elements $t>e$. A [value in a lattice-ordered group](../../../../../../value-in-a-lattice-ordered-group.md) of $t>e$ means a [convex lattice subgroup](../../../../../../convex-lattice-subgroup.md) maximal among those omitting $t$. Its [cover of a value in a lattice-ordered group](../../../../../../cover-of-a-value-in-a-lattice-ordered-group.md) will be denoted $V^*$: normal-valued means $V\triangleleft V^*$, not $V\triangleleft G$.

We first record facts about values and the coset order. [Zorn's lemma](../../../../../../zorn-s-lemma.md) supplies a value omitting any $t>e$, and supplies one containing any specified [convex lattice subgroup](../../../../../../convex-lattice-subgroup.md) that omits $t$. If $V$ is a value of $t$, every [convex lattice subgroup](../../../../../../convex-lattice-subgroup.md) strictly containing $V$ contains $t$. Therefore $V^*=\langle V,t\rangle_c$ is the least such subgroup and there are no intermediate convex lattice subgroups. Moreover, if $C\cap D=V$ and both strictly contain $V$, then both contain $t$, a contradiction. The criterion proved in part (i) thus makes $V$ a [prime convex lattice subgroup](../../../../../../prime-convex-lattice-subgroup.md): its right cosets are totally ordered. Equivalently, for $u,v\geq e$ with $u\wedge v=e$, at least one belongs to $V$. The equivalence follows because the coset projection preserves finite [meets](../../../../../../greatest-lower-bound-in-a-partially-ordered-set.md); in proving this, inequalities with two elements of $V$ can be replaced by their [join](../../../../../../least-upper-bound-in-a-partially-ordered-set.md).

The right-coset order gives the useful test

$$
Pu\leq Pv\iff (uv^{-1})\vee e\in P.\qquad\text{(2)}
$$

Indeed, $u\leq pv$ gives $(uv^{-1})\vee e\leq p\vee e\in P$, and [convexity](../../../../../../convex-function.md) gives membership. Conversely the displayed positive part itself supplies such a $p$. We will also use the basic [lattice-ordered group](../../../../../../lattice-ordered-group.md) identity that $(r\vee e)\wedge(r^{-1}\vee e)=e$: the positive and negative parts of one element are disjoint.

Here is a [squared bound from comparison at values](../../../../../../squared-bound-from-comparison-at-values.md). Suppose $p,q,x\geq e$ and $Vpq\geq Vx$ for every value $V$ of $x$. Then $p^2q^2\geq x$. To prove it, put

$$
d=(xq^{-2}p^{-2})\vee e
$$

and suppose $d>e$. Choose a value $P$ of $d$. If $x\in P$, then $e\leq d\leq x$, so $d\in P$, a contradiction. Otherwise extend $P$ to a value $V$ of $x$.

If $p\notin V$, set $c=(xq^{-2}p^{-1})\vee e$. Since $pq^2\geq pq$ and $Vpq\geq Vx$, test (2) gives $c\in V$. The element $(pc^{-1})\vee e$ is outside $V$: membership would imply $e\leq p\leq ((pc^{-1})\vee e)c\in V$, contradicting $p\notin V$. It is consequently outside $P$. Its inverse positive part is

$$
(cp^{-1})\vee e=(xq^{-2}p^{-2})\vee e=d,
$$

because $p^{-1}\leq e$. These two positive parts have [meet](../../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) $e$, so primeness of $P$ forces $d\in P$, again a contradiction.

If $p\in V$, then $Vpq=Vq$, and $c=(xq^{-1})\vee e\in V$. Necessarily $q\notin V$, since otherwise $Vx\leq V$ would put $x$ in $V$. Hence $t=p^2q\notin V$. As before, $(tc^{-1})\vee e$ is outside $V$ and outside $P$, while its inverse positive part is

$$
(ct^{-1})\vee e=(xq^{-2}p^{-2})\vee e=d;
$$

here $t^{-1}\leq e$. Primeness again yields the contradiction $d\in P$. Thus $d=e$, proving the bound. This auxiliary argument uses no normality assumption.

**Suppose first that all values are normal in their covers.** Given $a,b\geq e$, put $x=ab$. If $x=e$, both factors are $e$ and (1) holds. Otherwise choose any value $V$ of $x$. Since $e\leq a,b\leq x$, both factors belong to $V^*$. The [quotient group](../../../../../../quotient-group.md) $V^*/V$ is a [linearly ordered group](../../../../../../linearly-ordered-group.md), because $V$ is prime and is normal in $V^*$. It has no nontrivial proper [convex subgroup of an ordered group](../../../../../../convex-subgroup-of-an-ordered-group.md), since such a subgroup would lift to an intermediate convex lattice subgroup between $V$ and $V^*$.

This quotient is an [Archimedean ordered group](../../../../../../archimedean-ordered-group.md). If $u>e$ and all powers $u^n$ were bounded by some $v$, the [principal convex lattice subgroup](../../../../../../principal-convex-lattice-subgroup.md) generated by $u$ would be a nontrivial proper subgroup: it cannot contain $v$, since $v\leq u^m$ would contradict $u^{m+1}\leq v$. That contradicts the preceding paragraph.

For completeness, [Archimedean linearly ordered groups are Abelian](../../../../../../archimedean-linearly-ordered-groups-are-abelian.md) by the following elementary argument. If there is a least positive element $s$, its powers are cofinal and every element lies between consecutive powers; absence of any element between $e$ and $s$ makes the group cyclic. Otherwise, for every $c>e$ there is $d>e$ with $d^2<c$: choose $e<s<r<c$ and put $d_0=rs^{-1}$. If $d_0^2<r$, use $d=d_0$; if not, multiplication of $d_0^2\geq r$ gives $s^2\leq r<c$, so use $d=s$. If positive $g,h$ did not commute, interchange them to have $gh<hg$ and put $c=(gh)^{-1}hg>e$. Choose $d^2<c$ and, by the [Archimedean property](../../../../../../archimedean-property.md), integers $m,n\geq0$ with $d^m\leq g<d^{m+1}$ and $d^n\leq h<d^{n+1}$. Two-sided order invariance gives

$$
hg<d^{m+n+2},\qquad hg=ghc\geq d^{m+n}c>d^{m+n+2},
$$

a contradiction. Arbitrary nonidentity elements can be replaced by their positive inverses without changing whether they commute. This proves commutativity without assuming the characterization being proved.

It follows that $Vba=Vab=Vx$. Apply the squared-bound lemma with $p=b$, $q=a$ and $x=ab$, for all values of this $x$. We obtain

$$
\boxed{ab\leq b^2a^2.}
$$

Taking $a=|f|$ and $b=|g|$ gives the required inequality.

**Conversely, assume (1).** We need [one-sided bounds for adjoining a positive element](../../../../../../one-sided-bounds-for-adjoining-a-positive-element.md). If $H$ is any [convex lattice subgroup](../../../../../../convex-lattice-subgroup.md) and $a\geq e$, then

$$
\begin{aligned}
\langle H,a\rangle_c
&=\{g:|g|\leq ha^n\text{ for some }h\in H_{\geq e},\ n\geq0\}\\
&=\{g:|g|\leq a^nh\text{ for some }h\in H_{\geq e},\ n\geq0\}.\qquad\text{(3)}
\end{aligned}
$$

For the first equality, denote the indicated set by $S$. The inequality (1) allows a positive power of $a$ to move past a positive element of $H$, at the cost of squaring:

$$
(ha^n)(ka^m)\leq hk^2a^{2n+m}\qquad(h,k\in H_{\geq e}).
$$

Also $xy\leq|x||y|$ and $(xy)^{-1}\leq|y||x|$. Applying the bound in both orders, and taking the [join](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) of the two resulting elements of $H$ and the larger exponent, bounds $|xy|$ in the same form. Inversion does not change $|g|$. A common bound obtained from $h\vee k$ and the larger exponent proves closure under [join](../../../../../../least-upper-bound-in-a-partially-ordered-set.md), [meet](../../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) and order intervals. Thus $S$ is a [convex lattice subgroup](../../../../../../convex-lattice-subgroup.md) containing $H$ and $a$. Conversely every such subgroup contains each $ha^n$ and everything whose absolute value it bounds, proving equality. The same proof in the opposite group proves the second equality, since (1) with the variables interchanged reads $ba\leq a^2b^2$.

Let $V$ now be any value and $W=V^*$. For each $a\in W_{\geq e}\setminus V$, the subgroup $\langle V,a\rangle_c$ strictly contains $V$ and is contained in $W$, so the cover property makes it equal to $W$. Formula (3) therefore gives [power cofinality in the cover of a value](../../../../../../power-cofinality-in-the-cover-of-a-value.md): for every $b\in W_{\geq e}$ there are powers with

$$
Vb\leq Va^n,\qquad bV\leq a^mV.\qquad\text{(4)}
$$

Here the left cosets carry the order obtained by inversion from the right-coset order; equivalently $bV\leq a^mV$ means $b\leq a^mv$ for some $v\in V$.

Take $v\in V_{\geq e}$ and $a\in W_{\geq e}\setminus V$. If $u=a^{-1}va\notin V$, then $u\in W_{\geq e}\setminus V$ and

$$
au^n=v^na,\qquad Vu^n\leq Vau^n=Va\quad(n\geq1).
$$

The inequality uses $a\geq e$. But (4), applied to $u$ and the target $a^2$, gives $Va^2\leq Vu^n$ for some $n$. This contradicts $Va<Va^2$; equality of those two cosets would itself imply $a\in V$. Hence $a^{-1}va\in V$.

To obtain the other inclusion, suppose $w=ava^{-1}\notin V$. Then

$$
w^na=av^n,\qquad w^nV\leq w^naV=aV.
$$

Left-coset cofinality in (4) gives $a^2V\leq w^nV$, contradicting $aV<a^2V$. Thus $ava^{-1}\in V$ too. Every element of $V$ is a quotient of its two nonnegative lattice parts, so both conjugation inclusions hold for all $v\in V$. Positive elements of $W$ lying in $V$ already normalize $V$, and every element of $W$ is a quotient of two nonnegative elements. Consequently

$$
\boxed{V\triangleleft V^*.}
$$

All values have this property, so $G$ is normal-valued. At no stage was normality in the whole group assumed or required.

Finally, in a [linearly ordered group](../../../../../../linearly-ordered-group.md), nonnegative $a,b$ are comparable. If $a\leq b$, then $ab\leq b^2\leq b^2a^2$; if $b\leq a$, then $ab\leq a^2\leq b^2a^2$. Thus (1) holds in every o-group. The proved converse gives **every o-group is normal-valued**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
