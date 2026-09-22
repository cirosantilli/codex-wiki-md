<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Set $S=R\setminus P$, a [multiplicative subset](../../../../../multiplicatively-closed-set.md). The [localization at a prime ideal](../../../../../localization-at-a-prime-ideal.md) is $R_P=S^{-1}R$, whose elements are fractions $r/s$. Equality of two fractions means that $u(rs'-r's)=0$ for some $u\in S$. Likewise the [localization of a module](../../../../../localization-of-a-module.md) is $M_P=S^{-1}M$, with

$$
\frac m s=\frac{m'}{s'}\quad\Longleftrightarrow\quad u(s'm-sm')=0\text{ for some }u\in S.
$$

Addition uses a common denominator, and the [module](../../../../../module-mathematics.md) action is

$$
\boxed{\frac r s\,\frac m t=\frac{rm}{st}.}
$$

The equivalence relations make these operations well-defined, so $M_P$ is an $R_P$-module.

If $M\neq0$, choose $0\neq m\in M$. Its [annihilator](../../../../../annihilator-ring-theory.md) is proper, so it lies in a [maximal ideal](../../../../../maximal-ideal.md) $P$. The element $m/1$ cannot vanish in $M_P$: vanishing would mean $sm=0$ for some $s\notin P$, contrary to $\operatorname{Ann}_R(m)\subseteq P$. The converse is immediate by localizing the zero [module](../../../../../module-mathematics.md). Thus

$$
\boxed{M=0\quad\Longleftrightarrow\quad M_P=0\text{ for every prime }P.}
$$

This proof of [localization detects zero elements](../../../../../localization-detects-zero-elements.md) actually applies to arbitrary [modules](../../../../../module-mathematics.md), without finite-generation or [Noetherian](../../../../../noetherian-ring.md) assumptions. We will use that extra generality for an [Ext functor](../../../../../ext-functor.md) [module](../../../../../module-mathematics.md) below.

An [injective module](../../../../../injective-module.md) $E$ has the extension property: for each inclusion $A\hookrightarrow B$, every map $A\to E$ extends to a map $B\to E$. Equivalently, $\operatorname{Hom}_R(-,E)$ is exact. A [projective module](../../../../../projective-module.md) $Q$ has the lifting property: for each surjection $B\twoheadrightarrow C$, every map $Q\to C$ lifts to $Q\to B$. Equivalently, $\operatorname{Hom}_R(Q,-)$ is exact, or $Q$ is a direct summand of a [free module](../../../../../free-module.md).

For the [local criterion for injectivity over a Noetherian ring](../../../../../local-criterion-for-injectivity-over-a-noetherian-ring.md), recall the [Baer criterion](../../../../../baer-criterion.md): $E$ is injective precisely when every map from an [ideal](../../../../../ideal.md) $J\subseteq R$ into $E$ extends to $R$. Through the [short exact sequence](../../../../../short-exact-sequence.md) $0\to J\to R\to R/J\to0$, this is equivalent to

$$
\operatorname{Ext}^1_R(R/J,E)=0\quad\text{for every ideal }J.
$$

We also need [localization of Ext over a Noetherian ring](../../../../../localization-of-ext-over-a-noetherian-ring.md). Because $R$ is [Noetherian](../../../../../noetherian-ring.md), the [module](../../../../../module-mathematics.md) $R/J$ has a free resolution with every term finitely generated: all successive kernels are finitely generated, so this can be built recursively. For a finite free term $F$, the natural map

$$
S^{-1}\operatorname{Hom}_R(F,M)\cong\operatorname{Hom}_{S^{-1}R}(S^{-1}F,S^{-1}M)
$$

is an isomorphism, as is clear from a finite basis. [Exactness of localization](../../../../../exactness-of-localization.md) lets us pass to cohomology of the Hom complex. Therefore

$$
\boxed{\bigl(\operatorname{Ext}^1_R(R/J,M)\bigr)_P\cong\operatorname{Ext}^1_{R_P}(R_P/JR_P,M_P).}
$$

This explains the finiteness hypothesis needed for the localization argument, rather than assuming that localization preserves injectivity automatically.

If $M$ is injective, the left-hand side vanishes for every $J$ and $P$. Every [ideal](../../../../../ideal.md) $L$ of $R_P$ is $JR_P$, where $J$ is its contraction to $R$: if $r/s\in L$, then $r/1=s(r/s)\in L$, and conversely localization of a member of the contraction stays in $L$. Hence all [ideal](../../../../../ideal.md) tests for $M_P$ vanish, and the [Baer criterion](../../../../../baer-criterion.md) over $R_P$ makes $M_P$ injective.

Conversely, suppose every $M_P$ is injective. For each [ideal](../../../../../ideal.md) $J$, the displayed [Ext functor](../../../../../ext-functor.md) localization is zero at every prime. The zero-detection argument above gives $\operatorname{Ext}^1_R(R/J,M)=0$, without needing this Ext [module](../../../../../module-mathematics.md) to be finitely generated. Applying the [Baer criterion](../../../../../baer-criterion.md) over $R$ proves

$$
\boxed{M\text{ injective}\quad\Longleftrightarrow\quad M_P\text{ injective over }R_P\text{ for every prime }P.}
$$

In fact, under the [Noetherian](../../../../../noetherian-ring.md) [ring](../../../../../ring.md) hypothesis this equivalence holds for arbitrary $M$; the printed finite-generation assumption is more than is needed.

The [global dimension](../../../../../global-dimension.md) is

$$
\boxed{\operatorname{gldim}R=\sup\{\operatorname{pd}_R N:N\text{ an }R\text{-module}\},}
$$

where [projective dimension](../../../../../projective-dimension.md) is the smallest length of a [projective resolution](../../../../../projective-resolution.md), or infinity if there is no finite one. If $\operatorname{gldim}R=0$, every [module](../../../../../module-mathematics.md) is projective. Given an inclusion $A\hookrightarrow B$, the quotient $B/A$ is then projective, so the exact sequence $0\to A\to B\to B/A\to0$ splits. A retraction $\rho:B\to A$ exists. For any [module](../../../../../module-mathematics.md) $E$ and any map $f:A\to E$, the composition $f\rho:B\to E$ extends $f$. Thus every [module](../../../../../module-mathematics.md) is also injective. **Global dimension zero makes all [modules](../../../../../module-mathematics.md) both projective and injective**, as recorded by [global dimension zero and split exact sequences](../../../../../global-dimension-zero-and-split-exact-sequences.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
